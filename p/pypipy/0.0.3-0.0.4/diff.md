# Comparing `tmp/pypipy-0.0.3-py3-none-any.whl.zip` & `tmp/pypipy-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2286 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      202 b- defN 24-Apr-02 15:50 calc/calculator.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-Apr-02 15:51 pypipy-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      476 b- defN 24-Apr-02 15:51 pypipy-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 15:51 pypipy-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-02 15:51 pypipy-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      453 b- defN 24-Apr-02 15:51 pypipy-0.0.3.dist-info/RECORD
-6 files, 2317 bytes uncompressed, 1464 bytes compressed:  36.8%
+Zip file size: 2327 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      253 b- defN 24-Apr-03 01:48 calc/calculator.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      479 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      453 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/RECORD
+6 files, 2372 bytes uncompressed, 1505 bytes compressed:  36.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: calc/calculator.py
 Comment: 
 
-Filename: pypipy-0.0.3.dist-info/LICENSE
+Filename: pypipy-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pypipy-0.0.3.dist-info/METADATA
+Filename: pypipy-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pypipy-0.0.3.dist-info/WHEEL
+Filename: pypipy-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pypipy-0.0.3.dist-info/top_level.txt
+Filename: pypipy-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pypipy-0.0.3.dist-info/RECORD
+Filename: pypipy-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## calc/calculator.py

```diff
@@ -7,7 +7,11 @@
     for i in range(len(args)):
         result *= args[i]
     return result
 
 
 def aMinusB(a, b):
     return a - b
+
+
+def info():
+    print("나만의 패키지")
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pypipy-0.0.3.dist-info/LICENSE` & `pypipy-0.0.4.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

