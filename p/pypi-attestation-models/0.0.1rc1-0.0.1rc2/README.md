# Comparing `tmp/pypi_attestation_models-0.0.1rc1.tar.gz` & `tmp/pypi_attestation_models-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_attestation_models-0.0.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pypi_attestation_models-0.0.1rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypi_attestation_models-0.0.1rc1.tar` & `pypi_attestation_models-0.0.1rc2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10174 2024-05-02 21:30:31.898509 pypi_attestation_models-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0     1530 2024-05-02 21:30:31.898509 pypi_attestation_models-0.0.1rc1/README.md
--rw-r--r--   0        0        0     2744 2024-05-02 21:30:31.898509 pypi_attestation_models-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0      443 2024-05-02 21:30:31.898509 pypi_attestation_models-0.0.1rc1/src/pypi_attestation_models/__init__.py
--rw-r--r--   0        0        0     4151 2024-05-02 21:30:31.898509 pypi_attestation_models-0.0.1rc1/src/pypi_attestation_models/_impl.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 pypi_attestation_models-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0     2892 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/README.md
+-rw-r--r--   0        0        0     2766 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0      545 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/__init__.py
+-rw-r--r--   0        0        0     5886 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/_impl.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/py.typed
+-rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 pypi_attestation_models-0.0.1rc2/PKG-INFO
```

### Comparing `pypi_attestation_models-0.0.1rc1/LICENSE` & `pypi_attestation_models-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_attestation_models-0.0.1rc1/pyproject.toml` & `pypi_attestation_models-0.0.1rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 authors = [
     { name = "Trail of Bits", email = "opensource@trailofbits.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
-dependencies = ["cryptography", "pydantic", "sigstore==3.0.0rc1"]
+dependencies = ["cryptography", "pydantic", "sigstore==3.0.0rc2"]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 doc = ["pdoc"]
 test = ["pytest", "pytest-cov", "pretend", "coverage[toml]"]
 lint = [
     # NOTE: ruff is under active development, so we pin conservatively here
@@ -69,19 +69,19 @@
 
 [tool.ruff]
 line-length = 100
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["ALL"]
-# ANN102 is deprecated
+# ANN101 and ANN102 are deprecated
 # D203 and D213 are incompatible with D211 and D212 respectively.
 # COM812 and ISC001 can cause conflicts when using ruff as a formatter.
 # See https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules.
-ignore = ["ANN102", "D203", "D213", "COM812", "ISC001"]
+ignore = ["ANN101", "ANN102", "D203", "D213", "COM812", "ISC001"]
 
 [tool.ruff.lint.per-file-ignores]
 
 "test/**/*.py" = [
     "D",    # no docstrings in tests
     "S101", # asserts are expected in tests
 ]
```

### Comparing `pypi_attestation_models-0.0.1rc1/src/pypi_attestation_models/_impl.py` & `pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/_impl.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,36 +7,50 @@
 
 import binascii
 from base64 import b64decode, b64encode
 from hashlib import sha256
 from typing import TYPE_CHECKING, Annotated, Any, Literal, NewType
 
 import rfc8785
+import sigstore.errors
 from annotated_types import MinLen  # noqa: TCH002
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
 from pydantic import BaseModel
+from pydantic_core import ValidationError
 from sigstore.models import Bundle, LogEntry
 
 if TYPE_CHECKING:
     from pathlib import Path  # pragma: no cover
 
+    from sigstore.sign import Signer  # pragma: no cover
+    from sigstore.verify import Verifier  # pragma: no cover
+    from sigstore.verify.policy import VerificationPolicy  # pragma: no cover
+
 
 class ConversionError(ValueError):
     """The base error for all errors during conversion."""
 
 
 class InvalidAttestationError(ConversionError):
     """The PyPI Attestation given as input is not valid."""
 
     def __init__(self: InvalidAttestationError, msg: str) -> None:
         """Initialize an `InvalidAttestationError`."""
         super().__init__(f"Could not convert input Attestation: {msg}")
 
 
+class VerificationError(ValueError):
+    """The PyPI Attestation failed verification."""
+
+    def __init__(self: VerificationError, msg: str) -> None:
+        """Initialize an `VerificationError`."""
+        super().__init__(f"Verification failed: {msg}")
+
+
 TransparencyLogEntry = NewType("TransparencyLogEntry", dict[str, Any])
 
 
 class VerificationMaterial(BaseModel):
     """Cryptographic materials used to verify attestation objects."""
 
     certificate: str
@@ -66,14 +80,29 @@
 
     message_signature: str
     """
     The attestation's signature, as `base64(raw-sig)`, where `raw-sig`
     is the raw bytes of the signing operation over the attestation payload.
     """
 
+    def verify(self, verifier: Verifier, policy: VerificationPolicy, dist: Path) -> None:
+        """Verify against an existing Python artifact.
+
+        On failure, raises:
+        - `InvalidAttestationError` if the attestation could not be converted to
+           a Sigstore Bundle.
+        - `VerificationError` if the attestation could not be verified.
+        """
+        payload_to_verify = AttestationPayload.from_dist(dist)
+        bundle = pypi_to_sigstore(self)
+        try:
+            verifier.verify_artifact(bytes(payload_to_verify), bundle, policy)
+        except sigstore.errors.VerificationError as err:
+            raise VerificationError(str(err)) from err
+
 
 class AttestationPayload(BaseModel):
     """Attestation Payload object as defined in PEP 740."""
 
     distribution: str
     """
     The file name of the Python package distribution.
@@ -88,14 +117,19 @@
     def from_dist(cls, dist: Path) -> AttestationPayload:
         """Create an `AttestationPayload` from a distribution file."""
         return AttestationPayload(
             distribution=dist.name,
             digest=sha256(dist.read_bytes()).hexdigest(),
         )
 
+    def sign(self, signer: Signer) -> Attestation:
+        """Create a PEP 740 attestation by signing this payload."""
+        sigstore_bundle = signer.sign_artifact(bytes(self))
+        return sigstore_to_pypi(sigstore_bundle)
+
     def __bytes__(self: AttestationPayload) -> bytes:
         """Convert to bytes using a canonicalized JSON representation (from RFC8785)."""
         return rfc8785.dumps(self.model_dump())
 
 
 def sigstore_to_pypi(sigstore_bundle: Bundle) -> Attestation:
     """Convert a Sigstore Bundle into a PyPI attestation as defined in PEP 740."""
@@ -104,28 +138,37 @@
     )
 
     signature = sigstore_bundle._inner.message_signature.signature  # noqa: SLF001
     return Attestation(
         version=1,
         verification_material=VerificationMaterial(
             certificate=b64encode(certificate).decode("ascii"),
-            transparency_entries=[sigstore_bundle.log_entry._to_dict_rekor()],  # noqa: SLF001
+            transparency_entries=[TransparencyLogEntry(sigstore_bundle.log_entry._to_dict_rekor())],  # noqa: SLF001
         ),
         message_signature=b64encode(signature).decode("ascii"),
     )
 
 
 def pypi_to_sigstore(pypi_attestation: Attestation) -> Bundle:
     """Convert a PyPI attestation object as defined in PEP 740 into a Sigstore Bundle."""
     try:
         certificate_bytes = b64decode(pypi_attestation.verification_material.certificate)
         signature_bytes = b64decode(pypi_attestation.message_signature)
     except binascii.Error as err:
         raise InvalidAttestationError(str(err)) from err
 
     tlog_entry = pypi_attestation.verification_material.transparency_entries[0]
+    try:
+        certificate = x509.load_der_x509_certificate(certificate_bytes)
+    except ValueError as err:
+        raise InvalidAttestationError(str(err)) from err
+
+    try:
+        log_entry = LogEntry._from_dict_rekor(tlog_entry)  # noqa: SLF001
+    except (ValidationError, sigstore.errors.Error) as err:
+        raise InvalidAttestationError(str(err)) from err
 
     return Bundle.from_parts(
-        cert=x509.load_der_x509_certificate(certificate_bytes),
+        cert=certificate,
         sig=signature_bytes,
-        log_entry=LogEntry._from_dict_rekor(tlog_entry),  # noqa: SLF001
+        log_entry=log_entry,
     )
```

