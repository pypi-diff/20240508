# Comparing `tmp/bia_integrator_api-0.2.0.tar.gz` & `tmp/bia_integrator_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia_integrator_api-0.2.0.tar", max compression
+gzip compressed data, was "bia_integrator_api-0.3.0.tar", max compression
```

## Comparing `bia_integrator_api-0.2.0.tar` & `bia_integrator_api-0.3.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     8487 2023-12-05 11:38:35.644266 bia_integrator_api-0.2.0/Readme.md
--rw-r--r--   0        0        0     3940 2024-04-16 15:04:00.919705 bia_integrator_api-0.2.0/bia_integrator_api/__init__.py
--rw-r--r--   0        0        0      162 2024-04-16 15:04:00.923705 bia_integrator_api-0.2.0/bia_integrator_api/api/__init__.py
--rw-r--r--   0        0        0   242807 2024-04-16 15:04:00.867706 bia_integrator_api-0.2.0/bia_integrator_api/api/private_api.py
--rw-r--r--   0        0        0   114486 2024-04-16 15:04:00.895705 bia_integrator_api-0.2.0/bia_integrator_api/api/public_api.py
--rw-r--r--   0        0        0    30070 2024-04-16 15:04:00.931705 bia_integrator_api-0.2.0/bia_integrator_api/api_client.py
--rw-r--r--   0        0        0      844 2024-04-16 15:04:00.931705 bia_integrator_api-0.2.0/bia_integrator_api/api_response.py
--rw-r--r--   0        0        0    14696 2024-04-16 15:04:00.919705 bia_integrator_api-0.2.0/bia_integrator_api/configuration.py
--rw-r--r--   0        0        0      732 2023-12-05 11:38:35.644266 bia_integrator_api-0.2.0/bia_integrator_api/docs/Alias.md
--rw-r--r--   0        0        0      294 2024-04-16 15:04:00.179716 bia_integrator_api-0.2.0/bia_integrator_api/docs/AnnotationState.md
--rw-r--r--   0        0        0      985 2024-04-16 15:04:00.195716 bia_integrator_api-0.2.0/bia_integrator_api/docs/AuthenticationToken.md
--rw-r--r--   0        0        0      770 2024-04-16 15:04:00.207716 bia_integrator_api-0.2.0/bia_integrator_api/docs/Author.md
--rw-r--r--   0        0        0     1993 2024-04-16 15:04:00.223716 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIACollection.md
--rw-r--r--   0        0        0     2608 2024-04-16 15:04:00.239716 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImage.md
--rw-r--r--   0        0        0      982 2024-04-16 15:04:00.247715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageAlias.md
--rw-r--r--   0        0        0     1720 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageInput.md
--rw-r--r--   0        0        0     1245 2024-04-16 15:04:00.255715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageOmeMetadata.md
--rw-r--r--   0        0        0     1733 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageOutput.md
--rw-r--r--   0        0        0     1464 2024-04-16 15:04:00.263715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentation.md
--rw-r--r--   0        0        0     1527 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentationInput.md
--rw-r--r--   0        0        0     1540 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentationOutput.md
--rw-r--r--   0        0        0     2216 2024-04-16 15:04:00.275715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudy.md
--rw-r--r--   0        0        0     1554 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudyInput.md
--rw-r--r--   0        0        0     1567 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudyOutput.md
--rw-r--r--   0        0        0     2165 2024-04-16 15:04:00.287715 bia_integrator_api-0.2.0/bia_integrator_api/docs/Biosample.md
--rw-r--r--   0        0        0     1064 2024-04-16 15:04:00.299715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BiosampleAnnotation.md
--rw-r--r--   0        0        0      983 2024-04-16 15:04:00.311715 bia_integrator_api-0.2.0/bia_integrator_api/docs/BodyRegisterUser.md
--rw-r--r--   0        0        0     1478 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchFileReferencesExactMatch.md
--rw-r--r--   0        0        0     1001 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchImages.md
--rw-r--r--   0        0        0     1451 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchImagesExactMatch.md
--rw-r--r--   0        0        0     1313 2023-12-05 11:38:35.648266 bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchStudiesExactMatch.md
--rw-r--r--   0        0        0      992 2024-04-16 15:04:00.319714 bia_integrator_api-0.2.0/bia_integrator_api/docs/BulkOperationItem.md
--rw-r--r--   0        0        0     1091 2024-04-16 15:04:00.327714 bia_integrator_api-0.2.0/bia_integrator_api/docs/BulkOperationResponse.md
--rw-r--r--   0        0        0     1060 2024-04-16 15:04:00.343714 bia_integrator_api-0.2.0/bia_integrator_api/docs/ChannelRendering.md
--rw-r--r--   0        0        0     1077 2024-04-16 15:04:00.355714 bia_integrator_api-0.2.0/bia_integrator_api/docs/CollectionAnnotation.md
--rw-r--r--   0        0        0     1907 2024-04-16 15:04:00.367714 bia_integrator_api-0.2.0/bia_integrator_api/docs/FileReference.md
--rw-r--r--   0        0        0     1123 2024-04-16 15:04:00.379713 bia_integrator_api-0.2.0/bia_integrator_api/docs/FileReferenceAnnotation.md
--rw-r--r--   0        0        0     1006 2024-04-16 15:04:00.399713 bia_integrator_api-0.2.0/bia_integrator_api/docs/HTTPValidationError.md
--rw-r--r--   0        0        0     2093 2024-04-16 15:04:00.407713 bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAcquisition.md
--rw-r--r--   0        0        0     1162 2024-04-16 15:04:00.415713 bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAcquisitionAnnotation.md
--rw-r--r--   0        0        0     1012 2024-04-16 15:04:00.431712 bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAnnotation.md
--rw-r--r--   0        0        0      843 2024-04-16 15:04:00.443712 bia_integrator_api-0.2.0/bia_integrator_api/docs/LocationInner.md
--rw-r--r--   0        0        0      901 2024-04-16 15:04:00.451712 bia_integrator_api-0.2.0/bia_integrator_api/docs/ModelMetadata.md
--rw-r--r--   0        0        0      719 2024-04-16 15:04:00.467712 bia_integrator_api-0.2.0/bia_integrator_api/docs/Name.md
--rw-r--r--   0        0        0      885 2024-04-16 15:04:00.475712 bia_integrator_api-0.2.0/bia_integrator_api/docs/ObjectInfo.md
--rw-r--r--   0        0        0      926 2023-12-05 11:38:35.652266 bia_integrator_api-0.2.0/bia_integrator_api/docs/OmeMetadatSource.md
--rw-r--r--   0        0        0      869 2023-12-05 11:38:35.652266 bia_integrator_api-0.2.0/bia_integrator_api/docs/OriginalRelpath.md
--rw-r--r--   0        0        0      292 2024-04-16 15:04:00.479712 bia_integrator_api-0.2.0/bia_integrator_api/docs/OverwriteMode.md
--rw-r--r--   0        0        0    88028 2024-04-16 15:04:00.887705 bia_integrator_api-0.2.0/bia_integrator_api/docs/PrivateApi.md
--rw-r--r--   0        0        0    39419 2024-04-16 15:04:00.903705 bia_integrator_api-0.2.0/bia_integrator_api/docs/PublicApi.md
--rw-r--r--   0        0        0     1029 2024-04-16 15:04:00.491712 bia_integrator_api-0.2.0/bia_integrator_api/docs/RenderingInfo.md
--rw-r--r--   0        0        0     1035 2024-04-16 15:04:00.499711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchAnnotation.md
--rw-r--r--   0        0        0     1136 2024-04-16 15:04:00.503711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileReference.md
--rw-r--r--   0        0        0     1347 2024-04-16 15:04:00.511711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileReferenceFilter.md
--rw-r--r--   0        0        0     1165 2024-04-16 15:04:00.519711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileRepresentation.md
--rw-r--r--   0        0        0     1320 2024-04-16 15:04:00.527711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchImageFilter.md
--rw-r--r--   0        0        0     1158 2024-04-16 15:04:00.531711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchStudy.md
--rw-r--r--   0        0        0     1169 2024-04-16 15:04:00.539711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchStudyFilter.md
--rw-r--r--   0        0        0     1784 2024-04-16 15:04:00.547711 bia_integrator_api-0.2.0/bia_integrator_api/docs/Specimen.md
--rw-r--r--   0        0        0     1051 2024-04-16 15:04:00.555711 bia_integrator_api-0.2.0/bia_integrator_api/docs/SpecimenAnnotation.md
--rw-r--r--   0        0        0      791 2024-04-16 15:04:00.559711 bia_integrator_api-0.2.0/bia_integrator_api/docs/StartUuid.md
--rw-r--r--   0        0        0     1012 2024-04-16 15:04:00.563711 bia_integrator_api-0.2.0/bia_integrator_api/docs/StudyAnnotation.md
--rw-r--r--   0        0        0      791 2023-12-05 11:38:35.656266 bia_integrator_api-0.2.0/bia_integrator_api/docs/StudyUuid.md
--rw-r--r--   0        0        0      978 2024-04-16 15:04:00.571710 bia_integrator_api-0.2.0/bia_integrator_api/docs/ValidationError.md
--rw-r--r--   0        0        0     5345 2024-04-16 15:04:00.927705 bia_integrator_api-0.2.0/bia_integrator_api/exceptions.py
--rw-r--r--   0        0        0     3246 2024-04-16 15:04:00.923705 bia_integrator_api-0.2.0/bia_integrator_api/models/__init__.py
--rw-r--r--   0        0        0     3993 2023-12-05 11:38:35.660266 bia_integrator_api-0.2.0/bia_integrator_api/models/alias.py
--rw-r--r--   0        0        0      763 2024-04-16 15:04:00.175716 bia_integrator_api-0.2.0/bia_integrator_api/models/annotation_state.py
--rw-r--r--   0        0        0     2050 2024-04-16 15:04:00.191716 bia_integrator_api-0.2.0/bia_integrator_api/models/authentication_token.py
--rw-r--r--   0        0        0     1812 2024-04-16 15:04:00.203716 bia_integrator_api-0.2.0/bia_integrator_api/models/author.py
--rw-r--r--   0        0        0     5170 2024-04-16 15:04:00.219716 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_collection.py
--rw-r--r--   0        0        0     7155 2024-04-16 15:04:00.235716 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image.py
--rw-r--r--   0        0        0     1961 2024-04-16 15:04:00.243715 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_alias.py
--rw-r--r--   0        0        0     6189 2023-12-05 11:38:35.664265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_input.py
--rw-r--r--   0        0        0     3003 2024-04-16 15:04:00.251715 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_ome_metadata.py
--rw-r--r--   0        0        0     6196 2023-12-05 11:38:35.664265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_output.py
--rw-r--r--   0        0        0     3635 2024-04-16 15:04:00.259715 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation.py
--rw-r--r--   0        0        0     4198 2023-12-05 11:38:35.664265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation_input.py
--rw-r--r--   0        0        0     4205 2023-12-05 11:38:35.664265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation_output.py
--rw-r--r--   0        0        0     6782 2024-04-16 15:04:00.271715 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study.py
--rw-r--r--   0        0        0     7935 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study_input.py
--rw-r--r--   0        0        0     7943 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study_output.py
--rw-r--r--   0        0        0     5686 2024-04-16 15:04:00.283715 bia_integrator_api-0.2.0/bia_integrator_api/models/biosample.py
--rw-r--r--   0        0        0     2263 2024-04-16 15:04:00.291715 bia_integrator_api-0.2.0/bia_integrator_api/models/biosample_annotation.py
--rw-r--r--   0        0        0     2124 2024-04-16 15:04:00.303715 bia_integrator_api-0.2.0/bia_integrator_api/models/body_register_user.py
--rw-r--r--   0        0        0     4231 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_file_references_exact_match.py
--rw-r--r--   0        0        0     2303 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_images.py
--rw-r--r--   0        0        0     4516 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_images_exact_match.py
--rw-r--r--   0        0        0     3700 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_studies_exact_match.py
--rw-r--r--   0        0        0     2371 2024-04-16 15:04:00.315714 bia_integrator_api-0.2.0/bia_integrator_api/models/bulk_operation_item.py
--rw-r--r--   0        0        0     3139 2024-04-16 15:04:00.323714 bia_integrator_api-0.2.0/bia_integrator_api/models/bulk_operation_response.py
--rw-r--r--   0        0        0     2705 2024-04-16 15:04:00.343714 bia_integrator_api-0.2.0/bia_integrator_api/models/channel_rendering.py
--rw-r--r--   0        0        0     2271 2024-04-16 15:04:00.351714 bia_integrator_api-0.2.0/bia_integrator_api/models/collection_annotation.py
--rw-r--r--   0        0        0     4882 2024-04-16 15:04:00.367714 bia_integrator_api-0.2.0/bia_integrator_api/models/file_reference.py
--rw-r--r--   0        0        0     2295 2024-04-16 15:04:00.371713 bia_integrator_api-0.2.0/bia_integrator_api/models/file_reference_annotation.py
--rw-r--r--   0        0        0     2430 2024-04-16 15:04:00.395713 bia_integrator_api-0.2.0/bia_integrator_api/models/http_validation_error.py
--rw-r--r--   0        0        0     5240 2024-04-16 15:04:00.403713 bia_integrator_api-0.2.0/bia_integrator_api/models/image_acquisition.py
--rw-r--r--   0        0        0     2319 2024-04-16 15:04:00.411713 bia_integrator_api-0.2.0/bia_integrator_api/models/image_acquisition_annotation.py
--rw-r--r--   0        0        0     2231 2024-04-16 15:04:00.427713 bia_integrator_api-0.2.0/bia_integrator_api/models/image_annotation.py
--rw-r--r--   0        0        0     4676 2024-04-16 15:04:00.435712 bia_integrator_api-0.2.0/bia_integrator_api/models/location_inner.py
--rw-r--r--   0        0        0     1989 2024-04-16 15:04:00.447712 bia_integrator_api-0.2.0/bia_integrator_api/models/model_metadata.py
--rw-r--r--   0        0        0     3983 2024-04-16 15:04:00.463712 bia_integrator_api-0.2.0/bia_integrator_api/models/name.py
--rw-r--r--   0        0        0     2221 2024-04-16 15:04:00.471712 bia_integrator_api-0.2.0/bia_integrator_api/models/object_info.py
--rw-r--r--   0        0        0     1940 2023-12-05 11:38:35.668265 bia_integrator_api-0.2.0/bia_integrator_api/models/ome_metadat_source.py
--rw-r--r--   0        0        0     4093 2023-12-05 11:38:35.672265 bia_integrator_api-0.2.0/bia_integrator_api/models/original_relpath.py
--rw-r--r--   0        0        0      767 2024-04-16 15:04:00.475712 bia_integrator_api-0.2.0/bia_integrator_api/models/overwrite_mode.py
--rw-r--r--   0        0        0     3112 2024-04-16 15:04:00.487712 bia_integrator_api-0.2.0/bia_integrator_api/models/rendering_info.py
--rw-r--r--   0        0        0     3014 2024-04-16 15:04:00.495711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_annotation.py
--rw-r--r--   0        0        0     3478 2024-04-16 15:04:00.503711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_reference.py
--rw-r--r--   0        0        0     4172 2024-04-16 15:04:00.511711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_reference_filter.py
--rw-r--r--   0        0        0     3241 2024-04-16 15:04:00.515711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_representation.py
--rw-r--r--   0        0        0     4457 2024-04-16 15:04:00.523711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_image_filter.py
--rw-r--r--   0        0        0     4456 2024-04-16 15:04:00.531711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_study.py
--rw-r--r--   0        0        0     3633 2024-04-16 15:04:00.539711 bia_integrator_api-0.2.0/bia_integrator_api/models/search_study_filter.py
--rw-r--r--   0        0        0     4829 2024-04-16 15:04:00.543711 bia_integrator_api-0.2.0/bia_integrator_api/models/specimen.py
--rw-r--r--   0        0        0     2255 2024-04-16 15:04:00.551711 bia_integrator_api-0.2.0/bia_integrator_api/models/specimen_annotation.py
--rw-r--r--   0        0        0     4033 2024-04-16 15:04:00.559711 bia_integrator_api-0.2.0/bia_integrator_api/models/start_uuid.py
--rw-r--r--   0        0        0     2231 2024-04-16 15:04:00.563711 bia_integrator_api-0.2.0/bia_integrator_api/models/study_annotation.py
--rw-r--r--   0        0        0     4033 2023-12-05 11:38:35.672265 bia_integrator_api-0.2.0/bia_integrator_api/models/study_uuid.py
--rw-r--r--   0        0        0     2519 2024-04-16 15:04:00.567710 bia_integrator_api-0.2.0/bia_integrator_api/models/validation_error.py
--rw-r--r--   0        0        0    12919 2024-04-16 15:04:00.935705 bia_integrator_api-0.2.0/bia_integrator_api/rest.py
--rw-r--r--   0        0        0     3727 2024-04-16 14:46:55.479123 bia_integrator_api-0.2.0/bia_integrator_api/util.py
--rw-r--r--   0        0        0      462 2024-04-16 15:55:22.038959 bia_integrator_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9348 1970-01-01 00:00:00.000000 bia_integrator_api-0.2.0/setup.py
--rw-r--r--   0        0        0     8978 1970-01-01 00:00:00.000000 bia_integrator_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8487 2023-12-05 11:38:35.644266 bia_integrator_api-0.3.0/Readme.md
+-rw-r--r--   0        0        0     3940 2024-05-08 12:36:09.948258 bia_integrator_api-0.3.0/bia_integrator_api/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-07 10:25:48.901965 bia_integrator_api-0.3.0/bia_integrator_api/api/__init__.py
+-rw-r--r--   0        0        0   242659 2024-05-08 12:36:09.948258 bia_integrator_api-0.3.0/bia_integrator_api/api/private_api.py
+-rw-r--r--   0        0        0   114418 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/api/public_api.py
+-rw-r--r--   0        0        0    30070 2024-05-07 10:25:48.909965 bia_integrator_api-0.3.0/bia_integrator_api/api_client.py
+-rw-r--r--   0        0        0      844 2024-05-07 10:25:48.913965 bia_integrator_api-0.3.0/bia_integrator_api/api_response.py
+-rw-r--r--   0        0        0    14696 2024-05-07 10:25:48.897966 bia_integrator_api-0.3.0/bia_integrator_api/configuration.py
+-rw-r--r--   0        0        0      732 2023-12-05 11:38:35.644266 bia_integrator_api-0.3.0/bia_integrator_api/docs/Alias.md
+-rw-r--r--   0        0        0      294 2024-05-07 10:25:48.265970 bia_integrator_api-0.3.0/bia_integrator_api/docs/AnnotationState.md
+-rw-r--r--   0        0        0      985 2024-05-07 10:25:48.281970 bia_integrator_api-0.3.0/bia_integrator_api/docs/AuthenticationToken.md
+-rw-r--r--   0        0        0      770 2024-05-07 10:25:48.293970 bia_integrator_api-0.3.0/bia_integrator_api/docs/Author.md
+-rw-r--r--   0        0        0     1993 2024-05-07 10:25:48.309970 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIACollection.md
+-rw-r--r--   0        0        0     2608 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImage.md
+-rw-r--r--   0        0        0      982 2024-05-07 10:25:48.333970 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageAlias.md
+-rw-r--r--   0        0        0     1720 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageInput.md
+-rw-r--r--   0        0        0     1245 2024-05-07 10:25:48.345970 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageOmeMetadata.md
+-rw-r--r--   0        0        0     1733 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageOutput.md
+-rw-r--r--   0        0        0     1464 2024-05-07 10:25:48.353970 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentation.md
+-rw-r--r--   0        0        0     1527 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentationInput.md
+-rw-r--r--   0        0        0     1540 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentationOutput.md
+-rw-r--r--   0        0        0     2216 2024-05-07 10:25:48.365970 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudy.md
+-rw-r--r--   0        0        0     1554 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudyInput.md
+-rw-r--r--   0        0        0     1567 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudyOutput.md
+-rw-r--r--   0        0        0     2165 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/Biosample.md
+-rw-r--r--   0        0        0     1064 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/BiosampleAnnotation.md
+-rw-r--r--   0        0        0      983 2024-05-07 10:25:48.385969 bia_integrator_api-0.3.0/bia_integrator_api/docs/BodyRegisterUser.md
+-rw-r--r--   0        0        0     1478 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchFileReferencesExactMatch.md
+-rw-r--r--   0        0        0     1001 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchImages.md
+-rw-r--r--   0        0        0     1451 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchImagesExactMatch.md
+-rw-r--r--   0        0        0     1313 2023-12-05 11:38:35.648266 bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchStudiesExactMatch.md
+-rw-r--r--   0        0        0      992 2024-05-07 10:25:48.393969 bia_integrator_api-0.3.0/bia_integrator_api/docs/BulkOperationItem.md
+-rw-r--r--   0        0        0     1091 2024-05-07 10:25:48.397969 bia_integrator_api-0.3.0/bia_integrator_api/docs/BulkOperationResponse.md
+-rw-r--r--   0        0        0     1060 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/ChannelRendering.md
+-rw-r--r--   0        0        0     1077 2024-05-07 10:25:48.409969 bia_integrator_api-0.3.0/bia_integrator_api/docs/CollectionAnnotation.md
+-rw-r--r--   0        0        0     1907 2024-05-07 10:25:48.417969 bia_integrator_api-0.3.0/bia_integrator_api/docs/FileReference.md
+-rw-r--r--   0        0        0     1123 2024-05-07 10:25:48.421969 bia_integrator_api-0.3.0/bia_integrator_api/docs/FileReferenceAnnotation.md
+-rw-r--r--   0        0        0     1006 2024-05-07 10:25:48.429969 bia_integrator_api-0.3.0/bia_integrator_api/docs/HTTPValidationError.md
+-rw-r--r--   0        0        0     2093 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAcquisition.md
+-rw-r--r--   0        0        0     1162 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAcquisitionAnnotation.md
+-rw-r--r--   0        0        0     1012 2024-05-07 10:25:48.449969 bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAnnotation.md
+-rw-r--r--   0        0        0      843 2024-05-07 10:25:48.457969 bia_integrator_api-0.3.0/bia_integrator_api/docs/LocationInner.md
+-rw-r--r--   0        0        0      901 2024-05-07 10:25:48.465969 bia_integrator_api-0.3.0/bia_integrator_api/docs/ModelMetadata.md
+-rw-r--r--   0        0        0      719 2024-05-07 10:25:48.477969 bia_integrator_api-0.3.0/bia_integrator_api/docs/Name.md
+-rw-r--r--   0        0        0      885 2024-05-07 10:25:48.481969 bia_integrator_api-0.3.0/bia_integrator_api/docs/ObjectInfo.md
+-rw-r--r--   0        0        0      926 2023-12-05 11:38:35.652266 bia_integrator_api-0.3.0/bia_integrator_api/docs/OmeMetadatSource.md
+-rw-r--r--   0        0        0      869 2023-12-05 11:38:35.652266 bia_integrator_api-0.3.0/bia_integrator_api/docs/OriginalRelpath.md
+-rw-r--r--   0        0        0      292 2024-05-07 10:25:48.485969 bia_integrator_api-0.3.0/bia_integrator_api/docs/OverwriteMode.md
+-rw-r--r--   0        0        0    87880 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/PrivateApi.md
+-rw-r--r--   0        0        0    39351 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/PublicApi.md
+-rw-r--r--   0        0        0     1029 2024-05-07 10:25:48.493969 bia_integrator_api-0.3.0/bia_integrator_api/docs/RenderingInfo.md
+-rw-r--r--   0        0        0     1035 2024-05-07 10:25:48.497969 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchAnnotation.md
+-rw-r--r--   0        0        0     1136 2024-05-07 10:25:48.509969 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileReference.md
+-rw-r--r--   0        0        0     1347 2024-05-07 10:25:48.513969 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileReferenceFilter.md
+-rw-r--r--   0        0        0     1165 2024-05-07 10:25:48.521968 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileRepresentation.md
+-rw-r--r--   0        0        0     1320 2024-05-07 10:25:48.529968 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchImageFilter.md
+-rw-r--r--   0        0        0     1158 2024-05-07 10:25:48.533968 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchStudy.md
+-rw-r--r--   0        0        0     1169 2024-05-07 10:25:48.537968 bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchStudyFilter.md
+-rw-r--r--   0        0        0     1784 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/Specimen.md
+-rw-r--r--   0        0        0     1051 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/docs/SpecimenAnnotation.md
+-rw-r--r--   0        0        0      791 2024-05-07 10:25:48.557968 bia_integrator_api-0.3.0/bia_integrator_api/docs/StartUuid.md
+-rw-r--r--   0        0        0     1012 2024-05-07 10:25:48.565968 bia_integrator_api-0.3.0/bia_integrator_api/docs/StudyAnnotation.md
+-rw-r--r--   0        0        0      791 2023-12-05 11:38:35.656266 bia_integrator_api-0.3.0/bia_integrator_api/docs/StudyUuid.md
+-rw-r--r--   0        0        0      978 2024-05-07 10:25:48.597968 bia_integrator_api-0.3.0/bia_integrator_api/docs/ValidationError.md
+-rw-r--r--   0        0        0     5345 2024-05-07 10:25:48.905965 bia_integrator_api-0.3.0/bia_integrator_api/exceptions.py
+-rw-r--r--   0        0        0     3246 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/__init__.py
+-rw-r--r--   0        0        0     3993 2023-12-05 11:38:35.660266 bia_integrator_api-0.3.0/bia_integrator_api/models/alias.py
+-rw-r--r--   0        0        0      763 2024-05-07 10:25:48.261970 bia_integrator_api-0.3.0/bia_integrator_api/models/annotation_state.py
+-rw-r--r--   0        0        0     2050 2024-05-07 10:25:48.277970 bia_integrator_api-0.3.0/bia_integrator_api/models/authentication_token.py
+-rw-r--r--   0        0        0     1812 2024-05-07 10:25:48.289970 bia_integrator_api-0.3.0/bia_integrator_api/models/author.py
+-rw-r--r--   0        0        0     5170 2024-05-07 10:25:48.305970 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_collection.py
+-rw-r--r--   0        0        0     7155 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image.py
+-rw-r--r--   0        0        0     1961 2024-05-07 10:25:48.329970 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_alias.py
+-rw-r--r--   0        0        0     6189 2023-12-05 11:38:35.664265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_input.py
+-rw-r--r--   0        0        0     3003 2024-05-07 10:25:48.341970 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_ome_metadata.py
+-rw-r--r--   0        0        0     6196 2023-12-05 11:38:35.664265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_output.py
+-rw-r--r--   0        0        0     3635 2024-05-07 10:25:48.349970 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation.py
+-rw-r--r--   0        0        0     4198 2023-12-05 11:38:35.664265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation_input.py
+-rw-r--r--   0        0        0     4205 2023-12-05 11:38:35.664265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation_output.py
+-rw-r--r--   0        0        0     6782 2024-05-07 10:25:48.361970 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study.py
+-rw-r--r--   0        0        0     7935 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study_input.py
+-rw-r--r--   0        0        0     7943 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study_output.py
+-rw-r--r--   0        0        0     5686 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/biosample.py
+-rw-r--r--   0        0        0     2263 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/biosample_annotation.py
+-rw-r--r--   0        0        0     2124 2024-05-07 10:25:48.381970 bia_integrator_api-0.3.0/bia_integrator_api/models/body_register_user.py
+-rw-r--r--   0        0        0     4231 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_file_references_exact_match.py
+-rw-r--r--   0        0        0     2303 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_images.py
+-rw-r--r--   0        0        0     4516 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_images_exact_match.py
+-rw-r--r--   0        0        0     3700 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_studies_exact_match.py
+-rw-r--r--   0        0        0     2371 2024-05-07 10:25:48.389969 bia_integrator_api-0.3.0/bia_integrator_api/models/bulk_operation_item.py
+-rw-r--r--   0        0        0     3139 2024-05-07 10:25:48.397969 bia_integrator_api-0.3.0/bia_integrator_api/models/bulk_operation_response.py
+-rw-r--r--   0        0        0     2705 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/channel_rendering.py
+-rw-r--r--   0        0        0     2271 2024-05-07 10:25:48.409969 bia_integrator_api-0.3.0/bia_integrator_api/models/collection_annotation.py
+-rw-r--r--   0        0        0     4882 2024-05-07 10:25:48.413969 bia_integrator_api-0.3.0/bia_integrator_api/models/file_reference.py
+-rw-r--r--   0        0        0     2295 2024-05-07 10:25:48.421969 bia_integrator_api-0.3.0/bia_integrator_api/models/file_reference_annotation.py
+-rw-r--r--   0        0        0     2430 2024-05-07 10:25:48.425969 bia_integrator_api-0.3.0/bia_integrator_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     5240 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/image_acquisition.py
+-rw-r--r--   0        0        0     2319 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/image_acquisition_annotation.py
+-rw-r--r--   0        0        0     2231 2024-05-07 10:25:48.449969 bia_integrator_api-0.3.0/bia_integrator_api/models/image_annotation.py
+-rw-r--r--   0        0        0     4676 2024-05-07 10:25:48.457969 bia_integrator_api-0.3.0/bia_integrator_api/models/location_inner.py
+-rw-r--r--   0        0        0     1989 2024-05-07 10:25:48.465969 bia_integrator_api-0.3.0/bia_integrator_api/models/model_metadata.py
+-rw-r--r--   0        0        0     3983 2024-05-07 10:25:48.469969 bia_integrator_api-0.3.0/bia_integrator_api/models/name.py
+-rw-r--r--   0        0        0     2221 2024-05-07 10:25:48.481969 bia_integrator_api-0.3.0/bia_integrator_api/models/object_info.py
+-rw-r--r--   0        0        0     1940 2023-12-05 11:38:35.668265 bia_integrator_api-0.3.0/bia_integrator_api/models/ome_metadat_source.py
+-rw-r--r--   0        0        0     4093 2023-12-05 11:38:35.672265 bia_integrator_api-0.3.0/bia_integrator_api/models/original_relpath.py
+-rw-r--r--   0        0        0      767 2024-05-07 10:25:48.485969 bia_integrator_api-0.3.0/bia_integrator_api/models/overwrite_mode.py
+-rw-r--r--   0        0        0     3112 2024-05-07 10:25:48.493969 bia_integrator_api-0.3.0/bia_integrator_api/models/rendering_info.py
+-rw-r--r--   0        0        0     3014 2024-05-07 10:25:48.497969 bia_integrator_api-0.3.0/bia_integrator_api/models/search_annotation.py
+-rw-r--r--   0        0        0     3478 2024-05-07 10:25:48.505968 bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_reference.py
+-rw-r--r--   0        0        0     4172 2024-05-07 10:25:48.513969 bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_reference_filter.py
+-rw-r--r--   0        0        0     3241 2024-05-07 10:25:48.517969 bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_representation.py
+-rw-r--r--   0        0        0     4457 2024-05-07 10:25:48.525968 bia_integrator_api-0.3.0/bia_integrator_api/models/search_image_filter.py
+-rw-r--r--   0        0        0     4456 2024-05-07 10:25:48.529968 bia_integrator_api-0.3.0/bia_integrator_api/models/search_study.py
+-rw-r--r--   0        0        0     3633 2024-05-07 10:25:48.537968 bia_integrator_api-0.3.0/bia_integrator_api/models/search_study_filter.py
+-rw-r--r--   0        0        0     4829 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/specimen.py
+-rw-r--r--   0        0        0     2255 2024-05-08 12:36:09.952258 bia_integrator_api-0.3.0/bia_integrator_api/models/specimen_annotation.py
+-rw-r--r--   0        0        0     4033 2024-05-07 10:25:48.557968 bia_integrator_api-0.3.0/bia_integrator_api/models/start_uuid.py
+-rw-r--r--   0        0        0     2231 2024-05-07 10:25:48.561968 bia_integrator_api-0.3.0/bia_integrator_api/models/study_annotation.py
+-rw-r--r--   0        0        0     4033 2023-12-05 11:38:35.672265 bia_integrator_api-0.3.0/bia_integrator_api/models/study_uuid.py
+-rw-r--r--   0        0        0     2519 2024-05-07 10:25:48.597968 bia_integrator_api-0.3.0/bia_integrator_api/models/validation_error.py
+-rw-r--r--   0        0        0    12919 2024-05-07 10:25:48.917965 bia_integrator_api-0.3.0/bia_integrator_api/rest.py
+-rw-r--r--   0        0        0     3727 2024-04-19 16:41:30.403251 bia_integrator_api-0.3.0/bia_integrator_api/util.py
+-rw-r--r--   0        0        0      462 2024-05-08 12:36:09.984257 bia_integrator_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9348 1970-01-01 00:00:00.000000 bia_integrator_api-0.3.0/setup.py
+-rw-r--r--   0        0        0     8978 1970-01-01 00:00:00.000000 bia_integrator_api-0.3.0/PKG-INFO
```

### Comparing `bia_integrator_api-0.2.0/Readme.md` & `bia_integrator_api-0.3.0/Readme.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/__init__.py` & `bia_integrator_api-0.3.0/bia_integrator_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/api/private_api.py` & `bia_integrator_api-0.3.0/bia_integrator_api/api/private_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/biosamples', 'POST',
+            '/v1/private/biosamples', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -346,15 +346,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/collections', 'POST',
+            '/v1/private/collections', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -499,15 +499,15 @@
 
         _response_types_map = {
             '201': "BulkOperationResponse",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/file_references', 'POST',
+            '/v1/private/file_references', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -652,15 +652,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/image_acquisitions', 'POST',
+            '/v1/private/image_acquisitions', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -805,15 +805,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/images/{image_uuid}/representations/single', 'POST',
+            '/v1/private/images/{image_uuid}/representations/single', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -958,15 +958,15 @@
 
         _response_types_map = {
             '201': "BulkOperationResponse",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/images', 'POST',
+            '/v1/private/images', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1089,15 +1089,15 @@
         _auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
 
         _response_types_map = {
             '200': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/images/bulk', 'POST',
+            '/v1/private/images/bulk', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1242,15 +1242,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/specimens', 'POST',
+            '/v1/private/specimens', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1395,15 +1395,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/studies', 'POST',
+            '/v1/private/studies', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1533,15 +1533,15 @@
 
         _response_types_map = {
             '200': "Biosample",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/biosamples/{biosample_uuid}', 'GET',
+            '/v1/biosamples/{biosample_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1679,15 +1679,15 @@
 
         _response_types_map = {
             '200': "BIACollection",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/collections/{collection_uuid}', 'GET',
+            '/v1/collections/{collection_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1825,15 +1825,15 @@
 
         _response_types_map = {
             '200': "FileReference",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/file_references/{file_reference_uuid}', 'GET',
+            '/v1/file_references/{file_reference_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1971,15 +1971,15 @@
 
         _response_types_map = {
             '200': "BIAImage",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/images/{image_uuid}', 'GET',
+            '/v1/images/{image_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2109,15 +2109,15 @@
 
         _response_types_map = {
             '200': "ImageAcquisition",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/image_acquisitions/{image_acquisition_uuid}', 'GET',
+            '/v1/image_acquisitions/{image_acquisition_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2247,15 +2247,15 @@
 
         _response_types_map = {
             '200': "BIAImageOmeMetadata",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/images/{image_uuid}/ome_metadata', 'GET',
+            '/v1/images/{image_uuid}/ome_metadata', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2386,15 +2386,15 @@
 
         _response_types_map = {
             '200': "List[ObjectInfo]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/object_info_by_accessions', 'GET',
+            '/v1/object_info_by_accessions', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2524,15 +2524,15 @@
 
         _response_types_map = {
             '200': "Specimen",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/specimens/{specimen_uuid}', 'GET',
+            '/v1/specimens/{specimen_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2670,15 +2670,15 @@
 
         _response_types_map = {
             '200': "BIAStudy",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}', 'GET',
+            '/v1/studies/{study_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2834,15 +2834,15 @@
 
         _response_types_map = {
             '200': "List[FileReference]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}/file_references', 'GET',
+            '/v1/studies/{study_uuid}/file_references', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2998,15 +2998,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}/images', 'GET',
+            '/v1/studies/{study_uuid}/images', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3153,15 +3153,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_accession}/images_by_aliases', 'GET',
+            '/v1/studies/{study_accession}/images_by_aliases', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3282,15 +3282,15 @@
         _auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
 
         _response_types_map = {
             '200': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/admin/health-check', 'GET',
+            '/v1/admin/health-check', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3467,15 +3467,15 @@
 
         _response_types_map = {
             '200': "AuthenticationToken",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/auth/token', 'POST',
+            '/v1/auth/token', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3612,15 +3612,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/auth/users/register', 'POST',
+            '/v1/auth/users/register', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3758,15 +3758,15 @@
 
         _response_types_map = {
             '200': "List[BIACollection]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/collections', 'GET',
+            '/v1/collections', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -3913,15 +3913,15 @@
 
         _response_types_map = {
             '200': "List[FileReference]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/file_references/exact_match', 'POST',
+            '/v1/search/file_references/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4068,15 +4068,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/images/exact_match', 'POST',
+            '/v1/search/images/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4224,15 +4224,15 @@
 
         _response_types_map = {
             '200': "List[BIAStudy]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/studies', 'GET',
+            '/v1/search/studies', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4377,15 +4377,15 @@
 
         _response_types_map = {
             '200': "List[BIAStudy]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/studies/exact_match', 'POST',
+            '/v1/search/studies/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4530,15 +4530,15 @@
 
         _response_types_map = {
             '201': "BIAImageOmeMetadata",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/images/{image_uuid}/ome_metadata', 'POST',
+            '/v1/private/images/{image_uuid}/ome_metadata', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4670,15 +4670,15 @@
 
         _response_types_map = {
             '201': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/studies/{study_uuid}/refresh_counts', 'POST',
+            '/v1/private/studies/{study_uuid}/refresh_counts', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4815,15 +4815,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/biosamples', 'PATCH',
+            '/v1/private/biosamples', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -4960,15 +4960,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/file_references/single', 'PATCH',
+            '/v1/private/file_references/single', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -5107,15 +5107,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/images/single', 'PATCH',
+            '/v1/private/images/single', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -5252,15 +5252,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/image_acquisitions', 'PATCH',
+            '/v1/private/image_acquisitions', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -5397,15 +5397,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/specimens', 'PATCH',
+            '/v1/private/specimens', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -5542,15 +5542,15 @@
 
         _response_types_map = {
             '200': "object",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/private/studies', 'PATCH',
+            '/v1/private/studies', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/api/public_api.py` & `bia_integrator_api-0.3.0/bia_integrator_api/api/public_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
         _response_types_map = {
             '200': "Biosample",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/biosamples/{biosample_uuid}', 'GET',
+            '/v1/biosamples/{biosample_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -320,15 +320,15 @@
 
         _response_types_map = {
             '200': "BIACollection",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/collections/{collection_uuid}', 'GET',
+            '/v1/collections/{collection_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -466,15 +466,15 @@
 
         _response_types_map = {
             '200': "FileReference",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/file_references/{file_reference_uuid}', 'GET',
+            '/v1/file_references/{file_reference_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -612,15 +612,15 @@
 
         _response_types_map = {
             '200': "BIAImage",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/images/{image_uuid}', 'GET',
+            '/v1/images/{image_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -750,15 +750,15 @@
 
         _response_types_map = {
             '200': "ImageAcquisition",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/image_acquisitions/{image_acquisition_uuid}', 'GET',
+            '/v1/image_acquisitions/{image_acquisition_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -888,15 +888,15 @@
 
         _response_types_map = {
             '200': "BIAImageOmeMetadata",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/images/{image_uuid}/ome_metadata', 'GET',
+            '/v1/images/{image_uuid}/ome_metadata', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1027,15 +1027,15 @@
 
         _response_types_map = {
             '200': "List[ObjectInfo]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/object_info_by_accessions', 'GET',
+            '/v1/object_info_by_accessions', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1165,15 +1165,15 @@
 
         _response_types_map = {
             '200': "Specimen",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/specimens/{specimen_uuid}', 'GET',
+            '/v1/specimens/{specimen_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1311,15 +1311,15 @@
 
         _response_types_map = {
             '200': "BIAStudy",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}', 'GET',
+            '/v1/studies/{study_uuid}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1475,15 +1475,15 @@
 
         _response_types_map = {
             '200': "List[FileReference]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}/file_references', 'GET',
+            '/v1/studies/{study_uuid}/file_references', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1639,15 +1639,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_uuid}/images', 'GET',
+            '/v1/studies/{study_uuid}/images', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1794,15 +1794,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/studies/{study_accession}/images_by_aliases', 'GET',
+            '/v1/studies/{study_accession}/images_by_aliases', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1940,15 +1940,15 @@
 
         _response_types_map = {
             '200': "List[BIACollection]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/collections', 'GET',
+            '/v1/collections', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2095,15 +2095,15 @@
 
         _response_types_map = {
             '200': "List[FileReference]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/file_references/exact_match', 'POST',
+            '/v1/search/file_references/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2250,15 +2250,15 @@
 
         _response_types_map = {
             '200': "List[BIAImage]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/images/exact_match', 'POST',
+            '/v1/search/images/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2406,15 +2406,15 @@
 
         _response_types_map = {
             '200': "List[BIAStudy]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/studies', 'GET',
+            '/v1/search/studies', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2559,15 +2559,15 @@
 
         _response_types_map = {
             '200': "List[BIAStudy]",
             '422': "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/studies/exact_match', 'POST',
+            '/v1/search/studies/exact_match', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/api_client.py` & `bia_integrator_api-0.3.0/bia_integrator_api/api_client.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/api_response.py` & `bia_integrator_api-0.3.0/bia_integrator_api/api_response.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/configuration.py` & `bia_integrator_api-0.3.0/bia_integrator_api/configuration.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/Alias.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/Alias.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/AuthenticationToken.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/AuthenticationToken.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/Author.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/Author.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIACollection.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIACollection.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImage.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImage.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageAlias.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageAlias.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageInput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageInput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageOmeMetadata.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageOmeMetadata.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageOutput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageOutput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentationInput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentationInput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAImageRepresentationOutput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAImageRepresentationOutput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudy.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudy.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudyInput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudyInput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BIAStudyOutput.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BIAStudyOutput.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/Biosample.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/Biosample.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BiosampleAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BiosampleAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BodyRegisterUser.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BodyRegisterUser.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchFileReferencesExactMatch.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchFileReferencesExactMatch.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchImages.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchImages.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchImagesExactMatch.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchImagesExactMatch.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BodySearchStudiesExactMatch.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BodySearchStudiesExactMatch.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BulkOperationItem.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BulkOperationItem.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/BulkOperationResponse.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/BulkOperationResponse.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ChannelRendering.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ChannelRendering.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/CollectionAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/CollectionAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/FileReference.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/FileReference.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/FileReferenceAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/FileReferenceAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/HTTPValidationError.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/HTTPValidationError.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAcquisition.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAcquisition.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAcquisitionAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAcquisitionAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ImageAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ImageAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/LocationInner.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/LocationInner.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ModelMetadata.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ModelMetadata.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/Name.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/Name.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ObjectInfo.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ObjectInfo.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/OmeMetadatSource.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/OmeMetadatSource.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/OriginalRelpath.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/OriginalRelpath.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/PrivateApi.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/PrivateApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # bia_integrator_api.PrivateApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**create_biosample**](PrivateApi.md#create_biosample) | **POST** /api/v1/private/biosamples | Create Biosample
-[**create_collection**](PrivateApi.md#create_collection) | **POST** /api/v1/private/collections | Create Collection
-[**create_file_references**](PrivateApi.md#create_file_references) | **POST** /api/v1/private/file_references | Create File References
-[**create_image_acquisition**](PrivateApi.md#create_image_acquisition) | **POST** /api/v1/private/image_acquisitions | Create Image Acquisition
-[**create_image_representation**](PrivateApi.md#create_image_representation) | **POST** /api/v1/private/images/{image_uuid}/representations/single | Create Image Representation
-[**create_images**](PrivateApi.md#create_images) | **POST** /api/v1/private/images | Create Images
-[**create_images_bulk**](PrivateApi.md#create_images_bulk) | **POST** /api/v1/private/images/bulk | Create Images Bulk
-[**create_specimen**](PrivateApi.md#create_specimen) | **POST** /api/v1/private/specimens | Create Specimen
-[**create_study**](PrivateApi.md#create_study) | **POST** /api/v1/private/studies | Create Study
-[**get_biosample**](PrivateApi.md#get_biosample) | **GET** /api/v1/biosamples/{biosample_uuid} | Get Biosample
-[**get_collection**](PrivateApi.md#get_collection) | **GET** /api/v1/collections/{collection_uuid} | Get Collection
-[**get_file_reference**](PrivateApi.md#get_file_reference) | **GET** /api/v1/file_references/{file_reference_uuid} | Get File Reference
-[**get_image**](PrivateApi.md#get_image) | **GET** /api/v1/images/{image_uuid} | Get Image
-[**get_image_acquisition**](PrivateApi.md#get_image_acquisition) | **GET** /api/v1/image_acquisitions/{image_acquisition_uuid} | Get Image Acquisition
-[**get_image_ome_metadata**](PrivateApi.md#get_image_ome_metadata) | **GET** /api/v1/images/{image_uuid}/ome_metadata | Get Image Ome Metadata
-[**get_object_info_by_accession**](PrivateApi.md#get_object_info_by_accession) | **GET** /api/v1/object_info_by_accessions | Get Object Info By Accession
-[**get_specimen**](PrivateApi.md#get_specimen) | **GET** /api/v1/specimens/{specimen_uuid} | Get Specimen
-[**get_study**](PrivateApi.md#get_study) | **GET** /api/v1/studies/{study_uuid} | Get Study
-[**get_study_file_references**](PrivateApi.md#get_study_file_references) | **GET** /api/v1/studies/{study_uuid}/file_references | Get Study File References
-[**get_study_images**](PrivateApi.md#get_study_images) | **GET** /api/v1/studies/{study_uuid}/images | Get Study Images
-[**get_study_images_by_alias**](PrivateApi.md#get_study_images_by_alias) | **GET** /api/v1/studies/{study_accession}/images_by_aliases | Get Study Images By Alias
-[**health_check**](PrivateApi.md#health_check) | **GET** /api/v1/admin/health-check | Health Check
-[**login_for_access_token**](PrivateApi.md#login_for_access_token) | **POST** /api/v1/auth/token | Login For Access Token
-[**register_user**](PrivateApi.md#register_user) | **POST** /api/v1/auth/users/register | Register User
-[**search_collections**](PrivateApi.md#search_collections) | **GET** /api/v1/collections | Search Collections
-[**search_file_references_exact_match**](PrivateApi.md#search_file_references_exact_match) | **POST** /api/v1/search/file_references/exact_match | Search File References Exact Match
-[**search_images_exact_match**](PrivateApi.md#search_images_exact_match) | **POST** /api/v1/search/images/exact_match | Search Images Exact Match
-[**search_studies**](PrivateApi.md#search_studies) | **GET** /api/v1/search/studies | Search Studies
-[**search_studies_exact_match**](PrivateApi.md#search_studies_exact_match) | **POST** /api/v1/search/studies/exact_match | Search Studies Exact Match
-[**set_image_ome_metadata**](PrivateApi.md#set_image_ome_metadata) | **POST** /api/v1/private/images/{image_uuid}/ome_metadata | Set Image Ome Metadata
-[**study_refresh_counts**](PrivateApi.md#study_refresh_counts) | **POST** /api/v1/private/studies/{study_uuid}/refresh_counts | Study Refresh Counts
-[**update_biosample**](PrivateApi.md#update_biosample) | **PATCH** /api/v1/private/biosamples | Update Biosample
-[**update_file_reference**](PrivateApi.md#update_file_reference) | **PATCH** /api/v1/private/file_references/single | Update File Reference
-[**update_image**](PrivateApi.md#update_image) | **PATCH** /api/v1/private/images/single | Update Image
-[**update_image_acquisition**](PrivateApi.md#update_image_acquisition) | **PATCH** /api/v1/private/image_acquisitions | Update Image Acquisition
-[**update_specimen**](PrivateApi.md#update_specimen) | **PATCH** /api/v1/private/specimens | Update Specimen
-[**update_study**](PrivateApi.md#update_study) | **PATCH** /api/v1/private/studies | Update Study
+[**create_biosample**](PrivateApi.md#create_biosample) | **POST** /v1/private/biosamples | Create Biosample
+[**create_collection**](PrivateApi.md#create_collection) | **POST** /v1/private/collections | Create Collection
+[**create_file_references**](PrivateApi.md#create_file_references) | **POST** /v1/private/file_references | Create File References
+[**create_image_acquisition**](PrivateApi.md#create_image_acquisition) | **POST** /v1/private/image_acquisitions | Create Image Acquisition
+[**create_image_representation**](PrivateApi.md#create_image_representation) | **POST** /v1/private/images/{image_uuid}/representations/single | Create Image Representation
+[**create_images**](PrivateApi.md#create_images) | **POST** /v1/private/images | Create Images
+[**create_images_bulk**](PrivateApi.md#create_images_bulk) | **POST** /v1/private/images/bulk | Create Images Bulk
+[**create_specimen**](PrivateApi.md#create_specimen) | **POST** /v1/private/specimens | Create Specimen
+[**create_study**](PrivateApi.md#create_study) | **POST** /v1/private/studies | Create Study
+[**get_biosample**](PrivateApi.md#get_biosample) | **GET** /v1/biosamples/{biosample_uuid} | Get Biosample
+[**get_collection**](PrivateApi.md#get_collection) | **GET** /v1/collections/{collection_uuid} | Get Collection
+[**get_file_reference**](PrivateApi.md#get_file_reference) | **GET** /v1/file_references/{file_reference_uuid} | Get File Reference
+[**get_image**](PrivateApi.md#get_image) | **GET** /v1/images/{image_uuid} | Get Image
+[**get_image_acquisition**](PrivateApi.md#get_image_acquisition) | **GET** /v1/image_acquisitions/{image_acquisition_uuid} | Get Image Acquisition
+[**get_image_ome_metadata**](PrivateApi.md#get_image_ome_metadata) | **GET** /v1/images/{image_uuid}/ome_metadata | Get Image Ome Metadata
+[**get_object_info_by_accession**](PrivateApi.md#get_object_info_by_accession) | **GET** /v1/object_info_by_accessions | Get Object Info By Accession
+[**get_specimen**](PrivateApi.md#get_specimen) | **GET** /v1/specimens/{specimen_uuid} | Get Specimen
+[**get_study**](PrivateApi.md#get_study) | **GET** /v1/studies/{study_uuid} | Get Study
+[**get_study_file_references**](PrivateApi.md#get_study_file_references) | **GET** /v1/studies/{study_uuid}/file_references | Get Study File References
+[**get_study_images**](PrivateApi.md#get_study_images) | **GET** /v1/studies/{study_uuid}/images | Get Study Images
+[**get_study_images_by_alias**](PrivateApi.md#get_study_images_by_alias) | **GET** /v1/studies/{study_accession}/images_by_aliases | Get Study Images By Alias
+[**health_check**](PrivateApi.md#health_check) | **GET** /v1/admin/health-check | Health Check
+[**login_for_access_token**](PrivateApi.md#login_for_access_token) | **POST** /v1/auth/token | Login For Access Token
+[**register_user**](PrivateApi.md#register_user) | **POST** /v1/auth/users/register | Register User
+[**search_collections**](PrivateApi.md#search_collections) | **GET** /v1/collections | Search Collections
+[**search_file_references_exact_match**](PrivateApi.md#search_file_references_exact_match) | **POST** /v1/search/file_references/exact_match | Search File References Exact Match
+[**search_images_exact_match**](PrivateApi.md#search_images_exact_match) | **POST** /v1/search/images/exact_match | Search Images Exact Match
+[**search_studies**](PrivateApi.md#search_studies) | **GET** /v1/search/studies | Search Studies
+[**search_studies_exact_match**](PrivateApi.md#search_studies_exact_match) | **POST** /v1/search/studies/exact_match | Search Studies Exact Match
+[**set_image_ome_metadata**](PrivateApi.md#set_image_ome_metadata) | **POST** /v1/private/images/{image_uuid}/ome_metadata | Set Image Ome Metadata
+[**study_refresh_counts**](PrivateApi.md#study_refresh_counts) | **POST** /v1/private/studies/{study_uuid}/refresh_counts | Study Refresh Counts
+[**update_biosample**](PrivateApi.md#update_biosample) | **PATCH** /v1/private/biosamples | Update Biosample
+[**update_file_reference**](PrivateApi.md#update_file_reference) | **PATCH** /v1/private/file_references/single | Update File Reference
+[**update_image**](PrivateApi.md#update_image) | **PATCH** /v1/private/images/single | Update Image
+[**update_image_acquisition**](PrivateApi.md#update_image_acquisition) | **PATCH** /v1/private/image_acquisitions | Update Image Acquisition
+[**update_specimen**](PrivateApi.md#update_specimen) | **PATCH** /v1/private/specimens | Update Specimen
+[**update_study**](PrivateApi.md#update_study) | **PATCH** /v1/private/studies | Update Study
 
 
 # **create_biosample**
 > object create_biosample(biosample, overwrite_mode=overwrite_mode)
 
 Create Biosample
```

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/PublicApi.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/PublicApi.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # bia_integrator_api.PublicApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**get_biosample**](PublicApi.md#get_biosample) | **GET** /api/v1/biosamples/{biosample_uuid} | Get Biosample
-[**get_collection**](PublicApi.md#get_collection) | **GET** /api/v1/collections/{collection_uuid} | Get Collection
-[**get_file_reference**](PublicApi.md#get_file_reference) | **GET** /api/v1/file_references/{file_reference_uuid} | Get File Reference
-[**get_image**](PublicApi.md#get_image) | **GET** /api/v1/images/{image_uuid} | Get Image
-[**get_image_acquisition**](PublicApi.md#get_image_acquisition) | **GET** /api/v1/image_acquisitions/{image_acquisition_uuid} | Get Image Acquisition
-[**get_image_ome_metadata**](PublicApi.md#get_image_ome_metadata) | **GET** /api/v1/images/{image_uuid}/ome_metadata | Get Image Ome Metadata
-[**get_object_info_by_accession**](PublicApi.md#get_object_info_by_accession) | **GET** /api/v1/object_info_by_accessions | Get Object Info By Accession
-[**get_specimen**](PublicApi.md#get_specimen) | **GET** /api/v1/specimens/{specimen_uuid} | Get Specimen
-[**get_study**](PublicApi.md#get_study) | **GET** /api/v1/studies/{study_uuid} | Get Study
-[**get_study_file_references**](PublicApi.md#get_study_file_references) | **GET** /api/v1/studies/{study_uuid}/file_references | Get Study File References
-[**get_study_images**](PublicApi.md#get_study_images) | **GET** /api/v1/studies/{study_uuid}/images | Get Study Images
-[**get_study_images_by_alias**](PublicApi.md#get_study_images_by_alias) | **GET** /api/v1/studies/{study_accession}/images_by_aliases | Get Study Images By Alias
-[**search_collections**](PublicApi.md#search_collections) | **GET** /api/v1/collections | Search Collections
-[**search_file_references_exact_match**](PublicApi.md#search_file_references_exact_match) | **POST** /api/v1/search/file_references/exact_match | Search File References Exact Match
-[**search_images_exact_match**](PublicApi.md#search_images_exact_match) | **POST** /api/v1/search/images/exact_match | Search Images Exact Match
-[**search_studies**](PublicApi.md#search_studies) | **GET** /api/v1/search/studies | Search Studies
-[**search_studies_exact_match**](PublicApi.md#search_studies_exact_match) | **POST** /api/v1/search/studies/exact_match | Search Studies Exact Match
+[**get_biosample**](PublicApi.md#get_biosample) | **GET** /v1/biosamples/{biosample_uuid} | Get Biosample
+[**get_collection**](PublicApi.md#get_collection) | **GET** /v1/collections/{collection_uuid} | Get Collection
+[**get_file_reference**](PublicApi.md#get_file_reference) | **GET** /v1/file_references/{file_reference_uuid} | Get File Reference
+[**get_image**](PublicApi.md#get_image) | **GET** /v1/images/{image_uuid} | Get Image
+[**get_image_acquisition**](PublicApi.md#get_image_acquisition) | **GET** /v1/image_acquisitions/{image_acquisition_uuid} | Get Image Acquisition
+[**get_image_ome_metadata**](PublicApi.md#get_image_ome_metadata) | **GET** /v1/images/{image_uuid}/ome_metadata | Get Image Ome Metadata
+[**get_object_info_by_accession**](PublicApi.md#get_object_info_by_accession) | **GET** /v1/object_info_by_accessions | Get Object Info By Accession
+[**get_specimen**](PublicApi.md#get_specimen) | **GET** /v1/specimens/{specimen_uuid} | Get Specimen
+[**get_study**](PublicApi.md#get_study) | **GET** /v1/studies/{study_uuid} | Get Study
+[**get_study_file_references**](PublicApi.md#get_study_file_references) | **GET** /v1/studies/{study_uuid}/file_references | Get Study File References
+[**get_study_images**](PublicApi.md#get_study_images) | **GET** /v1/studies/{study_uuid}/images | Get Study Images
+[**get_study_images_by_alias**](PublicApi.md#get_study_images_by_alias) | **GET** /v1/studies/{study_accession}/images_by_aliases | Get Study Images By Alias
+[**search_collections**](PublicApi.md#search_collections) | **GET** /v1/collections | Search Collections
+[**search_file_references_exact_match**](PublicApi.md#search_file_references_exact_match) | **POST** /v1/search/file_references/exact_match | Search File References Exact Match
+[**search_images_exact_match**](PublicApi.md#search_images_exact_match) | **POST** /v1/search/images/exact_match | Search Images Exact Match
+[**search_studies**](PublicApi.md#search_studies) | **GET** /v1/search/studies | Search Studies
+[**search_studies_exact_match**](PublicApi.md#search_studies_exact_match) | **POST** /v1/search/studies/exact_match | Search Studies Exact Match
 
 
 # **get_biosample**
 > Biosample get_biosample(biosample_uuid)
 
 Get Biosample
```

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/RenderingInfo.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/RenderingInfo.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileReference.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileReference.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileReferenceFilter.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileReferenceFilter.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchFileRepresentation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchFileRepresentation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchImageFilter.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchImageFilter.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchStudy.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchStudy.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SearchStudyFilter.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SearchStudyFilter.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/Specimen.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/Specimen.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/SpecimenAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/SpecimenAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/StartUuid.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/StartUuid.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/StudyAnnotation.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/StudyAnnotation.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/StudyUuid.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/StudyUuid.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/docs/ValidationError.md` & `bia_integrator_api-0.3.0/bia_integrator_api/docs/ValidationError.md`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/exceptions.py` & `bia_integrator_api-0.3.0/bia_integrator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/__init__.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/alias.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/alias.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/annotation_state.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/annotation_state.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/authentication_token.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/authentication_token.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/author.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/author.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_collection.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_collection.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_alias.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_alias.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_input.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_input.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_ome_metadata.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_ome_metadata.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_output.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_output.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation_input.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation_input.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_image_representation_output.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_image_representation_output.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study_input.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study_input.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bia_study_output.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bia_study_output.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/biosample.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/biosample.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/biosample_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/biosample_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/body_register_user.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/body_register_user.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_file_references_exact_match.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_file_references_exact_match.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_images.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_images.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_images_exact_match.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_images_exact_match.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/body_search_studies_exact_match.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/body_search_studies_exact_match.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bulk_operation_item.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bulk_operation_item.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/bulk_operation_response.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/bulk_operation_response.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/channel_rendering.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/channel_rendering.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/collection_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/collection_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/file_reference.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/file_reference.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/file_reference_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/file_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/http_validation_error.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/image_acquisition.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/image_acquisition.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/image_acquisition_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/image_acquisition_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/image_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/image_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/location_inner.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/model_metadata.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/name.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/name.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/object_info.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/object_info.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/ome_metadat_source.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/ome_metadat_source.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/original_relpath.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/original_relpath.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/overwrite_mode.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/overwrite_mode.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/rendering_info.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/rendering_info.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_reference.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_reference.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_reference_filter.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_reference_filter.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_file_representation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_file_representation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_image_filter.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_image_filter.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_study.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_study.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/search_study_filter.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/search_study_filter.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/specimen.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/specimen.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/specimen_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/specimen_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/start_uuid.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/start_uuid.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/study_annotation.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/study_annotation.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/study_uuid.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/study_uuid.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/models/validation_error.py` & `bia_integrator_api-0.3.0/bia_integrator_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/rest.py` & `bia_integrator_api-0.3.0/bia_integrator_api/rest.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/bia_integrator_api/util.py` & `bia_integrator_api-0.3.0/bia_integrator_api/util.py`

 * *Files identical despite different names*

### Comparing `bia_integrator_api-0.2.0/setup.py` & `bia_integrator_api-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['aenum>=3.1.11',
  'pydantic>=1.10.5,<2.0.0',
  'python-dateutil>=2.8.2',
  'urllib3>=1.25.3']
 
 setup_kwargs = {
     'name': 'bia-integrator-api',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# BIA integrator API client\n\nThe [example](example/) project shows the most common operations that can be performed with the API.\n\nThe [generated documentation](bia_integrator_api_README.md#documentation-for-api-endpoints) is a full reference of all the functionality in the api client.\n\n⚠️**Important**⚠️\n* ⚠️ This client and some of the documentation are automatically generated, with some manual additions. This can lead to conflicting information. Please only use this Readme and the [example](example/) project for information, and everything else only as a reference. This Readme aims to separate the important/less important generated docs, so if something is unclear, suggestions for improving this file are welcome. \n* ⚠️ Because of the variety of usecases to accommotate, validations focus on maintaing db structure and some consistency but focus on flexibility. Please treat users with write access as you would a `root` user.\n\n## Notes on using the API\n\n### Read vs write client\n\nRead-only operations are generally public (unauthenticated) and read-write ones are private (authenticated). Two client classes exist, one for the public and one for the private modes of the API. This is mostly for editor support, since the private client includes all the public methods (and in addition to that, the write methods). This isn\'t done for read/write separation, so please use a single client throughout an app.\n\nBoth classes can be found [here](bia_integrator_api/api) and can be used as a reference. If using these as a reference, please ignore the methods with the `_with_http_info` suffix.\n\nAn alternative reference for the client methods is the [generated README](bia_integrator_api_README.md#documentation-for-api-endpoints), with methods tagged with their appropriate class.\n\n### Model hierarchy\n\nNested models are preferred and duplication is avoided, with exceptions where required. This results in a distinction between **toplevel** and **nested** objects.\n* **Toplevel** objects always have a `uuid` and `version` field, and they are one change unit most times (creating/updating objects only applies to them)\n* **Nested** objects never have the `uuid` and `version` fields, and are always nested in toplevel objects or other nested objects (eventually rooted in a toplevel object).\n\nIn the [example](./example/start_here.py) project (snippet below), `BIAStudy` is a toplevel object, and `Author` is nested in `BIAStudy`. Authors cannot be created independently, and in order to modify an author (or any nested/toplevel object) a push-update-pull for its root toplevel object must happen. The update will only be accepted if `version` is incremented.\n\n⚠️Note: `version` here is the object version, used to exclude concurrent writes. Type information, including version, is in the `model` attribute of all objects, managed by the server and should never be used or relied upon by client apps.\n\n```python\nmy_study = api_models.BIAStudy(\n    uuid = study_uuid,\n    version = 0,\n    title = "Study title",\n    description = "Study description",\n    release_date = "@TODO: Check format",\n    accession_id = f"accessions_must_be_unique_{study_uuid}",\n    organism = "test",\n    authors = [\n        api_models.Author(name="Study Author 1"),\n        api_models.Author(name="Study Author 2")\n    ]\n)\n```\n\nCurrently, `BIACollection`, `BIAStudy`, `BIAImage`, `FileReference` are toplevel objects, with everything else being nested. Some toplevel objects refer other objects, for example the BIAImage attribute `study_uuid` references the `uuid` field of a BIAStudy object. Generally, attributes named `TYPE_uuid` refer the `uuid` field of an object of that type.\n\n### Batch operations\n\nBulk creation is supported for objects of type `BIAImage` [create_images](bia_integrator_api/docs/PrivateApi.md#create_images) and `FileReference` [create_file_references](bia_integrator_api/docs/PrivateApi.md#create_file_references).\n\nThese endpoint always respond with a 201 status to avoid generated clients raising an exception, and return a [BulkOperationResponse](bia_integrator_api/docs/BulkOperationResponse.md) object with the actual result for each item written. **Individual writes are atomic** so if the BulkOperationResponseItem for a particular object has a 201 status, then it was written to the database, but **the operation as a wole is not atomic**. Some items might have been written and some might have failed, and the client must explicitly check if all items was written, and either do a partial or full retry (operations here are are idempotent, provided the documents being written are identical).\n\nThe `item_idx_by_status` attribute of BulkOperationResponse is a dictionary mapping the operation status (either 201 or 400) to the index of the document in the list passed to `create_images` (or `create_file_references`).\n\nPlease see the [example script](./example/start_here.py) for an example before using this.\n\n### Environments\n\nDevelopment is at https://bia-cron-1.ebi.ac.uk:8080/api/v1 available within the EBI network. User accounts are needed for write access. Read-only access is not authenticated.\n\nTo check the connection, install biaint using the project\'s [readme](../../tools/README.md) and list the available studies.\n\n### UUIDs\n\nBy design, models that require a UUID field expect them to be provided by the client generating the object. It is recommended that the UUIDs be deterministic, based on some important properties of the object being created.\n\nFor example, if FileReferences are created for files on a filesystem, the UUIDs could be derived from a mix of the absolute path of the files, and the file size (or its last modification time). This makes it easy to avoid duplicating a file if the operation of creating a large number of files fails halfway through, since the corresponding FileReferences would have the same UUID. Also, any stable identifier for the object being created can be used (e.g. the id in a legacy database)\n\nIn practise, this often looks similar to:\n\n```python\nobject_stable_attributes = {\n    \'stable_attribute_1\': attr_1,\n    \'stable_attribute_2\': attr_2\n}\nhash_input = json.dumps(object_stable_attributes, sort_keys=True)\nhexdigest = hashlib.md5(hash_input.encode("utf-8")).hexdigest()\nimage_id_as_uuid = uuid.UUID(version=4, hex=hexdigest)\n```\n\n### Write operations\n\nThere are two important things to consider when creating or modifying objects:\n\n1. Toplevel objects are versioned, and the versions need to be consecutive. When creating an object, its version must be set to 0, and then when modifications are made the version needs to be incremented. **Gotcha:** Providing an incorrect version when updating currently results in a "Not found" error instead of a conflict.\n2. Object creation and modification are idempotent. This is to simplify retries if deterministic UUIDs were used, because the objects that were created in the previous run are ignored.\n\n### Basic search\n\nThe API supports some basic search operations, aimed at simple usecases like "Which images in this study have representations bigger than 10TB?", "Which images have thumbnails", etc. Keep in mind that:\n* Queries are at the Image/Study/FileReference level, and they return the entire toplevel object. For example, if looking for all thumbnails in a study, a query for ImageRepresentions of type "thumbnail" would return *all BIAImage objects which have at least one thumbnail ImageRepresentation". The actual thumbnail ImageRepresentation needs to be extracted separately. \n* Although not required, queries for Images/FileReferences should **always** include the study uuid, to limit the search space. Queries currently timeout after 2 seconds.\n\nIn the API client, methods with names like `search_*` can be used for searching. See https://bia-cron-1.ebi.ac.uk:8080/redoc#tag/public/operation/search_images_exact_match an below for a reference of possible filters.\n\n**Example** body for a raw HTTP post. Client arguments are usually wrapped in `*Search` types. See the [search example](./example/image_search.py) for the api client equivalent.\n```json\n{\n    "annotations_any": [{"dimension_order": "XYZCT"} ],\n    "image_representations_any": [{"type": "thumbnail", "size_lte": 1000000000} ],\n    "study_uuid": "00000000-0000-0000-0006-09b5dbf57bdf",\n    "limit": 10\n}\n```\n\n\n## Setup\n\n`poetry add bia-integrator-api git+https://github.com/BioImage-Archive/bia-integrator.git@biaint-api-backend#subdirectory=clients/python`\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bia_integrator_api-0.2.0/PKG-INFO` & `bia_integrator_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-integrator-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.11)
```

