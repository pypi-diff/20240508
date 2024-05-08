# Comparing `tmp/virtualmachine-1.2.1.tar.gz` & `tmp/virtualmachine-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualmachine-1.2.1.tar", last modified: Thu Feb  1 12:57:44 2024, max compression
+gzip compressed data, was "virtualmachine-1.3.1.tar", last modified: Wed May  8 12:35:33 2024, max compression
```

## Comparing `virtualmachine-1.2.1.tar` & `virtualmachine-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/configure.ac
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.333687 virtualmachine-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.333687 virtualmachine-1.2.1/src/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/src/include/private/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/include/private/python.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/src/include/vmdetect/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/include/vmdetect/defs.h
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/include/vmdetect/virtualmachine.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/src/libvmdetect/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/libvmdetect/common.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.333687 virtualmachine-1.2.1/src/libvmdetect/os/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/src/libvmdetect/os/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/libvmdetect/os/linux/virtualmachine.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/src/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/python/get.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/src/python/init.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 12:57:44.337687 virtualmachine-1.2.1/virtualmachine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/virtualmachine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/virtualmachine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/virtualmachine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-01 12:57:44.000000 virtualmachine-1.2.1/virtualmachine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/private/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/private/python.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/vmdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/vmdetect/defs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/vmdetect/virtualmachine.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/libvmdetect/common.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/os/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/os/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/libvmdetect/os/linux/virtualmachine.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/python/get.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/python/init.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/virtualmachine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/top_level.txt
```

### Comparing `virtualmachine-1.2.1/LICENSE` & `virtualmachine-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/PKG-INFO` & `virtualmachine-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtualmachine
-Version: 1.2.1
+Version: 1.3.1
 Summary: Python library to identify virtual machine.
 Home-page: https://github.com/PerryWerneck/vmdetect
 Author: Perry Werneck
 Author-email: perry.werneck@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `virtualmachine-1.2.1/README.md` & `virtualmachine-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/configure.ac` & `virtualmachine-1.3.1/configure.ac`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dnl Process this file with autoconf to produce a configure script.
 
 dnl The minimum version of autoconf required.
 AC_PREREQ(2.59)
 
 dnl Initialise automake with the package name, version and
 dnl bug-reporting address.
-AC_INIT([vmdetect], [1.2], [perry.werneck@gmail.com], [vmdetect], [https://github.com/PerryWerneck/vmdetect.git])
+AC_INIT([vmdetect], [1.3], [perry.werneck@gmail.com], [vmdetect], [https://github.com/PerryWerneck/vmdetect.git])
 
 dnl Place auxilliary scripts here.
 AC_CONFIG_AUX_DIR([scripts])
 
 dnl Compute the canonical host-system type
 AC_CANONICAL_HOST
 
@@ -121,14 +121,22 @@
 dnl ---------------------------------------------------------------------------
 
 PKG_CHECK_MODULES( [SYSTEMD], [libsystemd], AC_DEFINE(HAVE_SYSTEMD,[],[Do we have systemd?]), AC_MSG_NOTICE([libsystemd not present.]) )
 AC_SUBST(SYSTEMD_CFLAGS)
 AC_SUBST(SYSTEMD_LIBS)
 
 dnl ---------------------------------------------------------------------------
+dnl Check for libdbus
+dnl ---------------------------------------------------------------------------
+
+dnl PKG_CHECK_MODULES( [DBUS], [dbus-1], AC_DEFINE(HAVE_DBUS,[],[Do we have d-bus?]), AC_MSG_NOTICE([ No DBUS support.]) )
+AC_SUBST(DBUS_LIBS)
+AC_SUBST(DBUS_CFLAGS)
+
+dnl ---------------------------------------------------------------------------
 dnl Check for wmi++
 dnl ---------------------------------------------------------------------------
 
 PKG_CHECK_MODULES( [WMI], [wmi++], app_cv_wmi="yes", app_cv_wmi="no" )
 
 if test "$app_cv_wmi" == "yes"; then
```

### Comparing `virtualmachine-1.2.1/setup.py` & `virtualmachine-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/src/include/private/python.h` & `virtualmachine-1.3.1/src/include/private/python.h`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/src/include/vmdetect/defs.h` & `virtualmachine-1.3.1/src/include/vmdetect/defs.h`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/src/include/vmdetect/virtualmachine.h` & `virtualmachine-1.3.1/src/include/vmdetect/virtualmachine.h`

 * *Files 13% similar despite different names*

```diff
@@ -25,16 +25,30 @@
 
  #include <string>
  #include <cstdint>
 
  extern "C" {
 
  class VMDETECT_API VirtualMachine {
+ private:
+	bool console_output = false;
+
  public:
 
+ 	constexpr VirtualMachine(bool v = false) : console_output{v} {
+ 	}
+
+ 	inline bool verbose() const noexcept {
+		return console_output;
+ 	}
+
+ 	inline void verbose(bool v) noexcept {
+		console_output = v;
+ 	}
+
 	enum CpuID : uint8_t {
 		BARE_METAL,			///< @brief Running on bare metal
 		VMWARE,				///< @brief Running on VMWare
 		VPC,				///< @brief Running on Virtual PC
 		BHIVE,				///< @brief Running on BHIVE
 		XEN,				///< @brief Running on XEN
 		KVM,				///< @brief Running on KVM
@@ -46,19 +60,19 @@
 	};
 
  	CpuID id() const;
 
 	operator bool() const;
 	std::string name() const;
 
- #ifndef _MSC_VER
+#ifndef _MSC_VER
 	inline std::string to_string() const {
 		return name();
 	}
- #endif // !_MSC_VER
+#endif // !_MSC_VER
 
 	static const VirtualMachine & getInstance();
 
  private:
 	CpuID translate(const char *sig) const;
 
  };
```

### Comparing `virtualmachine-1.2.1/src/libvmdetect/common.cc` & `virtualmachine-1.3.1/src/libvmdetect/common.cc`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/src/libvmdetect/os/linux/virtualmachine.cc` & `virtualmachine-1.3.1/src/libvmdetect/os/linux/virtualmachine.cc`

 * *Files 8% similar despite different names*

```diff
@@ -43,31 +43,71 @@
  #endif // HAVE_CONFIG_H
 
  #include <stdexcept>
  #include <vmdetect/virtualmachine.h>
  #include <cstring>
  #include <string>
  #include <stdint.h>
+ #include <iostream>
 
  using namespace std;
 
  #ifdef HAVE_SYSTEMD
 	#include <systemd/sd-bus.h>
  #endif // HAVE_SYSTEMD
 
 /*---[ Implement ]----------------------------------------------------------------------------------*/
 
  std::string VirtualMachine::name() const {
 
 	// Reference: (https://www.freedesktop.org/software/systemd/man/org.freedesktop.systemd1.html)
 	string virtualization;
 
-#ifdef HAVE_SYSTEMD
-	sd_bus * bus = NULL;
-	if(sd_bus_default_system(&bus)) {
+#if defined(HAVE_SYSTEMD)
+
+	struct SystemBus {
+
+		bool verbose;
+		sd_bus *ptr = NULL;
+
+		SystemBus(bool v) : verbose{v} {
+			int rc = sd_bus_default_system(&ptr);
+			if(rc < 0) {
+				if(verbose) {
+					cout << PACKAGE_NAME << "\tError " << rc << " getting system bus" << endl;
+				}
+				ptr = NULL;
+			}
+			if(verbose) {
+				cout << PACKAGE_NAME << "\tGot system bus on socket " << sd_bus_get_fd(ptr) << endl;
+			}
+		}
+
+		~SystemBus() {
+
+			sd_bus_flush(ptr);
+
+			if(verbose) {
+				cout << PACKAGE_NAME << "\tReleasing system bus from socket " << sd_bus_get_fd(ptr) << endl;
+			}
+
+			sd_bus_unrefp(&ptr);
+		}
+
+	};
+
+	struct BusMessage {
+		sd_bus_message *ptr = NULL;
+		~BusMessage() {
+			sd_bus_message_unrefp(&ptr);
+		}
+	};
+
+	SystemBus bus{console_output};
+	if(bus.ptr) {
 
 		try {
 
 			/*
 				dbus-send \
 					--session \
 					--dest=org.freedesktop.systemd1 \
@@ -75,56 +115,50 @@
 					"/org/freedesktop/systemd1" \
 					"org.freedesktop.DBus.Properties.Get" \
 					string:"org.freedesktop.systemd1.Manager" \
 					string:"Virtualization"
 			*/
 
 			sd_bus_error error = SD_BUS_ERROR_NULL;
-			sd_bus_message *response = NULL;
+			BusMessage response;
 
 			int rc = sd_bus_call_method(
-					bus,                   					// On the System Bus
+					bus.ptr,                   				// On the System Bus
 					"org.freedesktop.systemd1",				// Service to contact
 					"/org/freedesktop/systemd1", 			// Object path
 					"org.freedesktop.DBus.Properties",		// Interface name
 					"Get",									// Method to be called
 					&error,									// object to return error
-					&response,								// Response message on success
+					&response.ptr,							// Response message on success
 					"ss",
 					"org.freedesktop.systemd1.Manager",
 					"Virtualization"
 			);
 
 			if(rc < 0) {
 				string err = error.message;
 				sd_bus_error_free(&error);
 				throw runtime_error(err);;
 
-			} else if(response) {
+			} else if(response.ptr) {
 
 				char *text = NULL;
 
-				if(sd_bus_message_read(response, "v", "s", &text) < 0) {
-					sd_bus_message_unref(response);
+				if(sd_bus_message_read(response.ptr, "v", "s", &text) < 0) {
 					throw runtime_error("Can't parse systemd virtualization response");
 				} else if(text && *text) {
 					virtualization = text;
 				}
 
-				sd_bus_message_unref(response);
-
 			}
 
 		} catch(...) {
-			sd_bus_flush_close_unref(bus);
 			throw;
 		}
 
-		sd_bus_flush_close_unref(bus);
-
 		return virtualization;
 
 	}
 #endif // HAVE_SYSTEMD
 
 	// Cant get from SystemD, fallback
```

### Comparing `virtualmachine-1.2.1/src/python/get.cc` & `virtualmachine-1.3.1/src/python/get.cc`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/src/python/init.c` & `virtualmachine-1.3.1/src/python/init.c`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.2.1/virtualmachine.egg-info/PKG-INFO` & `virtualmachine-1.3.1/virtualmachine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtualmachine
-Version: 1.2.1
+Version: 1.3.1
 Summary: Python library to identify virtual machine.
 Home-page: https://github.com/PerryWerneck/vmdetect
 Author: Perry Werneck
 Author-email: perry.werneck@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

