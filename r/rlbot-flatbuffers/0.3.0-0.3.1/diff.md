# Comparing `tmp/rlbot_flatbuffers-0.3.0.tar.gz` & `tmp/rlbot_flatbuffers-0.3.1.tar.gz`

## Comparing `rlbot_flatbuffers-0.3.0.tar` & `rlbot_flatbuffers-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.0/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/LICENSE
--rw-r--r--   0     1001      127      479 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/README.md
--rw-r--r--   0     1001      127    57972 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/build.rs
--rw-r--r--   0     1001      127      182 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/README.md
--rw-r--r--   0     1001      127     2661 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/comms.fbs
--rw-r--r--   0     1001      127     1932 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/event.fbs
--rwxr-xr-x   0     1001      127  6681832 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc
--rw-r--r--   0     1001      127  3488256 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc.exe
--rw-r--r--   0     1001      127  6896752 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc_mac
--rw-r--r--   0     1001      127     1281 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/gamestate.fbs
--rw-r--r--   0     1001      127     5824 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/matchstart.fbs
--rw-r--r--   0     1001      127     1162 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/rendering.fbs
--rw-r--r--   0     1001      127     6275 2024-03-26 22:42:41.000000 rlbot_flatbuffers-0.3.0/flatbuffers-schema/rlbot.fbs
--rw-r--r--   0     1001      127     4624 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/src/lib.rs
--rw-r--r--   0     1001      127    12644 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/Cargo.lock
--rw-r--r--   0     1001      127      418 2024-03-26 22:42:40.000000 rlbot_flatbuffers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/LICENSE
+-rw-r--r--   0     1001      127      479 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/README.md
+-rw-r--r--   0     1001      127    60169 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/build.rs
+-rw-r--r--   0     1001      127      182 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/README.md
+-rw-r--r--   0     1001      127      401 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/comms.fbs
+-rw-r--r--   0     1001      127     1932 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/event.fbs
+-rwxr-xr-x   0     1001      127  6681832 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc
+-rw-r--r--   0     1001      127  3488256 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc.exe
+-rw-r--r--   0     1001      127  6896752 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc_mac
+-rw-r--r--   0     1001      127     1281 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/gamestate.fbs
+-rw-r--r--   0     1001      127     5824 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/matchstart.fbs
+-rw-r--r--   0     1001      127     1162 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/rendering.fbs
+-rw-r--r--   0     1001      127     6296 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/rlbot.fbs
+-rw-r--r--   0     1001      127     4770 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      127    12644 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/Cargo.lock
+-rw-r--r--   0     1001      127      418 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.1/PKG-INFO
```

### Comparing `rlbot_flatbuffers-0.3.0/Cargo.toml` & `rlbot_flatbuffers-0.3.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlbot-flatbuffers-py"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 description = "A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers"
 repository = "https://github.com/VirxEC/rlbot-flatbuffers-py"
 license = "MIT"
 readme = "README.md"
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore", ".gitmodules"]
 publish = false
```

### Comparing `rlbot_flatbuffers-0.3.0/LICENSE` & `rlbot_flatbuffers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/build.rs` & `rlbot_flatbuffers-0.3.1/build.rs`

 * *Files 4% similar despite different names*

```diff
@@ -270,14 +270,16 @@
             let mut variable_type = variable_info[1].to_string();
 
             if variable_type.starts_with("Vec<") && variable_type.ends_with("T>") {
                 variable_type = format!(
                     "Vec<Py<super::{}>>",
                     variable_type.trim_start_matches("Vec<").trim_end_matches("T>")
                 );
+            } else if variable_type.starts_with("Vec<") && variable_type.ends_with('>') {
+                variable_type = String::from("Py<PyBytes>");
             } else if variable_type.starts_with("Box<") && variable_type.ends_with('>') {
                 variable_type = format!(
                     "Py<super::{}>",
                     variable_type
                         .trim_start_matches("Box<")
                         .trim_end_matches('>')
                         .trim_end_matches('T')
@@ -311,16 +313,19 @@
         self.write_str("        Py::new(py, Self {");
 
         for variable_info in &self.types {
             let variable_name = &variable_info[0];
             let variable_type = &variable_info[1];
 
             if variable_type.starts_with("Vec<") {
-                self.file_contents
-                    .push(Cow::Owned(format!("            {variable_name}: Vec::new(),")));
+                self.file_contents.push(Cow::Owned(if variable_type == "Vec<u8>" {
+                    format!("            {variable_name}: PyBytes::new_bound(py, &[]).unbind(),")
+                } else {
+                    format!("            {variable_name}: Vec::new(),")
+                }));
             } else if variable_type.starts_with("Option<") {
                 self.file_contents
                     .push(Cow::Owned(format!("            {variable_name}: None,")));
             } else if !Self::BASE_TYPES.contains(&variable_type.as_str())
                 && (variable_type.starts_with("Box<") || variable_type.ends_with('T'))
             {
                 let inner_type = variable_type
@@ -491,27 +496,30 @@
             self.write_string(format!("        Py::new(py, {} {{", self.struct_name));
 
             for variable_info in &self.types {
                 let variable_name = &variable_info[0];
                 let variable_type = variable_info[1].as_str();
 
                 if variable_type.starts_with("Vec<") {
-                    let inner_type = variable_type.trim_start_matches("Vec<").trim_end_matches('>');
-                    if Self::BASE_TYPES.contains(&inner_type) {
-                        self.file_contents
-                            .push(Cow::Owned(format!("            {variable_name}: flat_t.{variable_name},")));
+                    self.file_contents
+                            .push(Cow::Owned(if variable_type == "Vec<u8>" {
+                        format!("            {variable_name}: PyBytes::new_bound(py, &flat_t.{variable_name}).unbind(),")
                     } else {
-                        self.file_contents.push(Cow::Owned(format!(
+                        format!(
                             "            {variable_name}: flat_t.{variable_name}.into_iter().map(|x| x.into_gil(py)).collect(),",
-                        )));
-                    }
+                        )
+                    }));
                 } else if variable_type.starts_with("Option<") {
-                    self.file_contents.push(Cow::Owned(format!(
-                        "            {variable_name}: flat_t.{variable_name}.map(|x| x.into_gil(py)),",
-                    )));
+                    self.file_contents.push(Cow::Owned(
+                        if variable_type.trim_start_matches("Option<").trim_end_matches('>') == "String" {
+                            format!("            {variable_name}: flat_t.{variable_name},")
+                        } else {
+                            format!("            {variable_name}: flat_t.{variable_name}.map(|x| x.into_gil(py)),")
+                        },
+                    ));
                 } else if variable_type.starts_with("Box<") || variable_type.ends_with('T') {
                     self.file_contents.push(Cow::Owned(format!(
                         "            {variable_name}: flat_t.{variable_name}.into_gil(py),",
                     )));
                 } else if Self::BASE_TYPES.contains(&variable_type) {
                     self.file_contents
                         .push(Cow::Owned(format!("            {variable_name}: flat_t.{variable_name},")));
@@ -638,27 +646,33 @@
                 self.write_str("        Self {");
 
                 for variable_info in &self.types {
                     let variable_name = &variable_info[0];
                     let variable_type = variable_info[1].as_str();
 
                     if variable_type.starts_with("Vec<") {
-                        let inner_type = variable_type.trim_start_matches("Vec<").trim_end_matches('>');
-                        if Self::BASE_TYPES.contains(&inner_type) {
-                            self.file_contents
-                                .push(Cow::Owned(format!("            {variable_name}: py_type.{variable_name},")));
+                        self.file_contents.push(Cow::Owned(if variable_type == "Vec<u8>" {
+                            format!(
+                                "            {variable_name}: py_type.{variable_name}.as_bytes(py).to_vec(),"
+                            )
                         } else {
-                            self.file_contents.push(Cow::Owned(format!(
+                            format!(
                                 "            {variable_name}: py_type.{variable_name}.iter().map(|x| x.into_gil(py)).collect(),",
-                            )));
-                        }
+                            )
+                        }));
                     } else if variable_type.starts_with("Option<") {
-                        self.file_contents.push(Cow::Owned(format!(
-                            "            {variable_name}: py_type.{variable_name}.as_ref().map(|x| x.into_gil(py)),",
-                        )));
+                        self.file_contents.push(Cow::Owned(
+                            if variable_type.trim_start_matches("Option<").trim_end_matches('>') == "String" {
+                                format!("            {variable_name}: py_type.{variable_name}.clone(),")
+                            } else {
+                                format!(
+                                    "            {variable_name}: py_type.{variable_name}.as_ref().map(|x| x.into_gil(py)),"
+                                )
+                            },
+                        ));
                     } else if variable_type == "String" {
                         self.file_contents.push(Cow::Owned(format!(
                             "            {variable_name}: py_type.{variable_name}.clone(),",
                         )));
                     } else if variable_type.ends_with('T') || variable_type.starts_with("Box<") {
                         self.file_contents.push(Cow::Owned(format!(
                             "            {variable_name}: (&py_type.{variable_name}).into_gil(py),",
@@ -698,27 +712,33 @@
                 }
 
                 for variable_info in &self.types {
                     let variable_name = &variable_info[0];
                     let variable_type = variable_info[1].as_str();
 
                     if variable_type.starts_with("Vec<") {
-                        let inner_type = variable_type.trim_start_matches("Vec<").trim_end_matches('>');
-                        if Self::BASE_TYPES.contains(&inner_type) {
-                            self.file_contents
-                                .push(Cow::Owned(format!("            {variable_name}: borrow.{variable_name},")));
+                        if variable_type == "Vec<u8>" {
+                            self.file_contents.push(Cow::Owned(format!(
+                                "            {variable_name}: borrow.{variable_name}.as_bytes(py).to_vec(),"
+                            )));
                         } else {
                             self.file_contents.push(Cow::Owned(format!(
                                 "            {variable_name}: borrow.{variable_name}.iter().map(|x| x.into_gil(py)).collect(),",
                             )));
                         }
                     } else if variable_type.starts_with("Option<") {
-                        self.file_contents.push(Cow::Owned(format!(
-                            "            {variable_name}: borrow.{variable_name}.as_ref().map(|x| x.into_gil(py)),",
-                        )));
+                        self.file_contents.push(Cow::Owned(
+                            if variable_type.trim_start_matches("Option<").trim_end_matches('>') == "String" {
+                                format!("            {variable_name}: borrow.{variable_name}.clone(),")
+                            } else {
+                                format!(
+                                    "            {variable_name}: borrow.{variable_name}.as_ref().map(|x| x.into_gil(py)),"
+                                )
+                            },
+                        ));
                     } else if variable_type == "String" {
                         self.file_contents.push(Cow::Owned(format!(
                             "            {variable_name}: borrow.{variable_name}.clone(),",
                         )));
                     } else if variable_type.ends_with('T') || variable_type.starts_with("Box<") {
                         self.file_contents.push(Cow::Owned(format!(
                             "            {variable_name}: (&borrow.{variable_name}).into_gil(py),",
@@ -841,14 +861,16 @@
                 }
 
                 signature_parts.push(format!("{variable_name}=None"));
             } else if !Self::BASE_TYPES.contains(&variable_type.as_str())
                 && (variable_type.starts_with("Box<") || variable_type.ends_with('T'))
             {
                 signature_parts.push(format!("{variable_name}=crate::get_py_default()"));
+            } else if variable_type == "Vec<u8>" {
+                signature_parts.push(format!("{variable_name}=crate::get_empty_pybytes()"));
             } else {
                 signature_parts.push(format!("{variable_name}=Default::default()"));
             }
         }
 
         self.write_string(format!("    #[pyo3(signature = ({}))]", signature_parts.join(", ")));
         self.write_str("    pub fn new(");
@@ -862,14 +884,16 @@
             let mut variable_type = variable_info[1].to_string();
 
             if variable_type.starts_with("Vec<") && variable_type.ends_with("T>") {
                 variable_type = format!(
                     "Vec<Py<super::{}>>",
                     variable_type.trim_start_matches("Vec<").trim_end_matches("T>")
                 );
+            } else if variable_type == "Vec<u8>" {
+                variable_type = String::from("Py<PyBytes>");
             } else if variable_type.starts_with("Box<") && variable_type.ends_with('>') {
                 variable_type = format!(
                     "Py<super::{}>",
                     variable_type
                         .trim_start_matches("Box<")
                         .trim_end_matches('>')
                         .trim_end_matches('T')
@@ -974,27 +998,29 @@
         if self.types.is_empty() {
             self.write_str("    pub fn __repr__(&self, _py: Python) -> String {");
             self.write_string(format!("        String::from(\"{}()\")", self.struct_name));
             self.write_str("    }");
             return;
         }
 
-        self.write_str("#[allow(unused_variables)]");
+        self.write_str("    #[allow(unused_variables)]");
         self.write_str("    pub fn __repr__(&self, py: Python) -> String {");
         self.write_str("        format!(");
 
         let repr_signature = self
             .types
             .iter()
             .map(|variable_info| {
                 let variable_name = &variable_info[0];
                 let variable_type = variable_info[1].as_str();
 
                 if variable_type == "String" {
                     format!("{variable_name}={{:?}}")
+                } else if variable_type == "Vec<u8>" {
+                    format!("{variable_name}=bytes([{{}}])")
                 } else if variable_type.starts_with("Vec<") {
                     format!("{variable_name}=[{{}}]")
                 } else {
                     format!("{variable_name}={{}}")
                 }
             })
             .collect::<Vec<_>>()
@@ -1011,24 +1037,36 @@
             } else if Self::BASE_TYPES.contains(&variable_type) {
                 self.file_contents
                     .push(Cow::Owned(format!("            self.{variable_name},")));
             } else if variable_type.starts_with("Option<") {
                 self.file_contents
                     .push(Cow::Owned(format!("            self.{variable_name}")));
                 self.file_contents.push(Cow::Borrowed("                .as_ref()"));
-                self.file_contents
-                    .push(Cow::Borrowed("                .map(|x| x.borrow(py).__repr__(py))"));
+                if Self::BASE_TYPES.into_iter().any(|t| variable_type.contains(t)) {
+                    self.file_contents
+                        .push(Cow::Borrowed("                .map(|i| format!(\"{i:?}\"))"));
+                } else {
+                    self.file_contents
+                        .push(Cow::Borrowed("                .map(|x| x.borrow(py).__repr__(py))"));
+                }
                 self.file_contents
                     .push(Cow::Borrowed("                .unwrap_or_else(crate::none_str),"));
             } else if variable_type.starts_with("Vec<") {
                 self.file_contents
                     .push(Cow::Owned(format!("            self.{variable_name}")));
-                self.file_contents.push(Cow::Borrowed("                .iter()"));
-                self.file_contents
-                    .push(Cow::Borrowed("                .map(|x| x.borrow(py).__repr__(py))"));
+                if Self::BASE_TYPES.into_iter().any(|t| variable_type.contains(t)) {
+                    self.file_contents.push(Cow::Borrowed("                .as_bytes(py)"));
+                    self.file_contents.push(Cow::Borrowed("                .iter()"));
+                    self.file_contents
+                        .push(Cow::Borrowed("                .map(ToString::to_string)"));
+                } else {
+                    self.file_contents.push(Cow::Borrowed("                .iter()"));
+                    self.file_contents
+                        .push(Cow::Borrowed("                .map(|x| x.borrow(py).__repr__(py))"));
+                }
                 self.file_contents
                     .push(Cow::Borrowed("                .collect::<Vec<String>>()"));
                 self.file_contents.push(Cow::Borrowed("                .join(\", \"),"));
             } else if variable_type.ends_with('T') || variable_type.starts_with("Box<") {
                 self.file_contents.push(Cow::Owned(format!(
                     "            self.{variable_name}.borrow(py).__repr__(py),"
                 )));
@@ -1192,14 +1230,15 @@
     let primitive_map = [
         ("bool", "bool"),
         ("i32", "int"),
         ("u32", "int"),
         ("f32", "float"),
         ("String", "str"),
         ("u8", "int"),
+        ("Vec<u8>", "bytes"),
     ];
 
     for (_, type_name, types) in type_data {
         let is_enum = !types.is_empty()
             && types
                 .iter()
                 .enumerate()
@@ -1322,14 +1361,15 @@
 
                     let variable_type = variable_info[1].clone();
 
                     let default_value = match variable_type.as_str() {
                         "bool" => Cow::Borrowed("False"),
                         "i32" | "u32" | "f32" | "u8" => Cow::Borrowed("0"),
                         "String" => Cow::Borrowed("\"\""),
+                        "Vec<u8>" => Cow::Borrowed("b\"\""),
                         t => {
                             if t.starts_with("Vec<") {
                                 Cow::Borrowed("[]")
                             } else if t.starts_with("Box<") {
                                 let inner_type = t.trim_start_matches("Box<").trim_end_matches('>').trim_end_matches('T');
                                 Cow::Owned(format!("{inner_type}()"))
                             } else if t.starts_with("Option<") {
```

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/event.fbs` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/event.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc.exe` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc.exe`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/flatc_mac` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc_mac`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/gamestate.fbs` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/gamestate.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/matchstart.fbs` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/matchstart.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/rendering.fbs` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/rendering.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.0/flatbuffers-schema/rlbot.fbs` & `rlbot_flatbuffers-0.3.1/flatbuffers-schema/rlbot.fbs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+include "comms.fbs";
 include "event.fbs";
 include "gamestate.fbs";
 include "matchstart.fbs";
 include "rendering.fbs";
 
 namespace rlbot.flat;
```

### Comparing `rlbot_flatbuffers-0.3.0/src/lib.rs` & `rlbot_flatbuffers-0.3.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     unused_imports
 )]
 pub mod generated;
 
 #[allow(clippy::enum_variant_names)]
 mod python;
 
-use pyo3::{prelude::*, PyClass};
+use pyo3::{prelude::*, types::PyBytes, PyClass};
 use python::*;
 
 pub trait FromGil<T> {
     fn from_gil(py: Python, obj: T) -> Self;
 }
 
 pub trait IntoGil<T>: Sized {
@@ -39,14 +39,18 @@
 
 impl<T: Default + PyClass + Into<PyClassInitializer<T>>> PyDefault for T {
     fn py_default(py: Python) -> Py<Self> {
         Py::new(py, Self::default()).unwrap()
     }
 }
 
+pub fn get_empty_pybytes() -> Py<PyBytes> {
+    Python::with_gil(|py| PyBytes::new_bound(py, &[]).unbind())
+}
+
 pub fn get_py_default<T: PyDefault>() -> Py<T> {
     Python::with_gil(|py| T::py_default(py))
 }
 
 #[must_use]
 pub fn none_str() -> String {
     String::from("None")
@@ -116,97 +120,98 @@
     };
 }
 
 pynamedmodule! {
     doc: "rlbot_flatbuffers is a Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers.",
     name: rlbot_flatbuffers,
     classes: [
-        MessagePacket,
-        PredictionSlice,
-        SphereShape,
-        PartyMember,
-        GameMode,
-        Physics,
+        ExistingMatchBehavior,
         PlayerStatEvent,
-        RenderMessage,
-        GameStateType,
-        GameMessage,
+        MatchComm,
+        DesiredCarState,
+        RemoveRenderGroup,
         BallPrediction,
-        MutatorSettings,
-        Vector3,
-        RotatorPartial,
-        DesiredBallState,
-        PlayerInputChange,
-        BallSizeOption,
+        PlayerInfo,
+        GameStateType,
+        GameSpeedOption,
         ScoreInfo,
-        PlayerLoadout,
-        PlayerConfiguration,
-        BoostStrengthOption,
-        ReadyMessage,
-        Line3D,
-        PlayerClass,
-        CollisionShape,
-        Color,
-        Float,
-        MatchLength,
-        RLBot,
-        RemoveRenderGroup,
-        DesiredGameInfoState,
-        GravityOption,
-        Bool,
+        MessagePacket,
         DemolishOption,
-        GameTickPacket,
-        Psyonix,
-        GameMessageWrapper,
-        OvertimeOption,
-        BoostOption,
-        DesiredCarState,
         Vector3Partial,
-        PlayerSpectate,
-        AirState,
-        Launcher,
-        String3D,
+        TextHAlign,
+        BoostOption,
+        RumbleOption,
+        Vector3,
+        GravityOption,
         BallInfo,
-        ExistingMatchBehavior,
-        RenderGroup,
-        PlayerInput,
+        ReadyMessage,
         StartCommand,
-        FieldInfo,
+        MatchSettings,
+        OvertimeOption,
+        PlayerSpectate,
+        SphereShape,
+        Touch,
+        TextVAlign,
         ConsoleCommand,
-        SeriesLengthOption,
+        DesiredGameInfoState,
+        PredictionSlice,
+        PolyLine3D,
+        Rotator,
         BallTypeOption,
-        DesiredGameState,
-        String2D,
-        StopCommand,
-        DesiredBoostState,
-        Human,
-        DesiredPhysics,
-        ScriptConfiguration,
-        ControllerState,
+        LoadoutPaint,
+        RotatorPartial,
+        RLBot,
         CylinderShape,
+        PlayerInputChange,
+        DesiredBallState,
+        CollisionShape,
+        RenderMessage,
+        BoostPadState,
+        GameMode,
+        ControllerState,
+        BoostStrengthOption,
+        GoalInfo,
         BallBouncinessOption,
-        TeamInfo,
-        PolyLine3D,
+        MaxScore,
+        SeriesLengthOption,
+        GameMessage,
+        DesiredBoostState,
+        BallSizeOption,
+        BallMaxSpeedOption,
+        MatchLength,
         BallWeightOption,
-        LoadoutPaint,
-        BoxShape,
+        PlayerLoadout,
+        Psyonix,
+        DesiredPhysics,
+        AirState,
+        GameMessageWrapper,
+        GameTickPacket,
+        Human,
+        String3D,
+        Float,
+        FieldInfo,
+        PlayerClass,
         BoostPad,
-        MatchSettings,
-        BallMaxSpeedOption,
+        Bool,
+        RespawnTimeOption,
+        String2D,
+        PartyMember,
         GameInfo,
-        Touch,
-        RumbleOption,
-        TextVAlign,
+        StopCommand,
+        PlayerInput,
+        Color,
+        Line3D,
+        Physics,
+        MutatorSettings,
+        PlayerConfiguration,
+        DesiredGameState,
+        TeamInfo,
         RenderType,
-        GoalInfo,
-        TextHAlign,
-        GameSpeedOption,
-        MaxScore,
-        BoostPadState,
-        PlayerInfo,
-        RespawnTimeOption,
-        Rotator
+        RenderGroup,
+        ScriptConfiguration,
+        Launcher,
+        BoxShape
     ],
     vars: [
         ("__version__", env!("CARGO_PKG_VERSION"))
     ]
 }
```

### Comparing `rlbot_flatbuffers-0.3.0/Cargo.lock` & `rlbot_flatbuffers-0.3.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c124f12ade4e670107b132722d0ad1a5c9790bcbc1b265336369ea05626b4498"
 dependencies = [
  "attribute-derive-macro",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "attribute-derive-macro"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b217a07446e0fb086f83401a98297e2d81492122f5874db5391bd270a185f88"
@@ -23,15 +23,15 @@
  "collection_literals",
  "interpolator",
  "proc-macro-error",
  "proc-macro-utils",
  "proc-macro2",
  "quote",
  "quote-use",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -58,21 +58,21 @@
 name = "derive-where"
 version = "1.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62d671cc41a825ebabc75757b62d3d168c577f9149b2d49ece1dad1f72119d25"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "flatbuffers"
 version = "24.3.25"
-source = "git+https://github.com/google/flatbuffers?branch=master#8f2e1dbd88d25ca76cbcaf9ac8c9919e0a787d31"
+source = "git+https://github.com/google/flatbuffers?branch=master#f4a9c5325b7cba8ae432466bdfb90f857da0d593"
 dependencies = [
  "bitflags",
  "rustc_version",
 ]
 
 [[package]]
 name = "get-size"
@@ -87,15 +87,15 @@
 name = "get-size-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13a1bcfb855c1f340d5913ab542e36f25a1c56f57de79022928297632435dec2"
 dependencies = [
  "attribute-derive",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
@@ -214,17 +214,17 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -232,55 +232,55 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -292,41 +292,41 @@
 name = "quote-use"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7b5abe3fe82fdeeb93f44d66a7b444dedf2e4827defb0a8e69c437b2de2ef94"
 dependencies = [
  "quote",
  "quote-use-macros",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "quote-use-macros"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97ea44c7e20f16017a76a245bb42188517e13d16dcb1aa18044bc406cdc3f4af"
 dependencies = [
  "derive-where",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlbot-flatbuffers-py"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "flatbuffers",
  "get-size",
  "pyo3",
  "serde",
 ]
 
@@ -364,15 +364,15 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
@@ -385,17 +385,17 @@
 dependencies = [
  "proc-macro2",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `rlbot_flatbuffers-0.3.0/PKG-INFO` & `rlbot_flatbuffers-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlbot_flatbuffers
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers
 License: MIT
 Requires-Python: >=3.10
```

