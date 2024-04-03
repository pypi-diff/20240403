# Comparing `tmp/mathematical-expression-py-1.2.1.tar.gz` & `tmp/mathematical-expression-py-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathematical-expression-py-1.2.1.tar", last modified: Mon Jan  8 06:57:06 2024, max compression
+gzip compressed data, was "mathematical-expression-py-1.2.4.tar", last modified: Wed Apr  3 10:24:33 2024, max compression
```

## Comparing `mathematical-expression-py-1.2.1.tar` & `mathematical-expression-py-1.2.4.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:06.101565 mathematical-expression-py-1.2.1/
--rw-rw-rw-   0        0        0    11558 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    25835 2024-01-08 06:57:06.085943 mathematical-expression-py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    25198 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/README.md
--rw-rw-rw-   0        0        0      625 2024-01-08 06:35:24.000000 mathematical-expression-py-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-08 06:57:06.101565 mathematical-expression-py-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.393485 mathematical-expression-py-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.487979 mathematical-expression-py-1.2.1/src/mathematical_expression/
--rw-rw-rw-   0        0        0     2615 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.487979 mathematical-expression-py-1.2.1/src/mathematical_expression/core/
--rw-rw-rw-   0        0        0       51 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.560326 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/
--rw-rw-rw-   0        0        0     1616 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/Calculation.py
--rw-rw-rw-   0        0        0      843 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/SharedCalculation.py
--rw-rw-rw-   0        0        0       45 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.629744 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/__init__.py
--rw-rw-rw-   0        0        0     3060 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/booleanCalculation.py
--rw-rw-rw-   0        0        0     4326 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.645373 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/function/
--rw-rw-rw-   0        0        0     1194 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/function/Function.py
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/function/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.677639 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/bracketsCalculation.py
--rw-rw-rw-   0        0        0     4374 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py
--rw-rw-rw-   0        0        0     4336 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py
--rw-rw-rw-   0        0        0     2202 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py
--rw-rw-rw-   0        0        0     6380 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py
--rw-rw-rw-   0        0        0     6315 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py
--rw-rw-rw-   0        0        0     7863 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py
--rw-rw-rw-   0        0        0     3222 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/numberCalculation.py
--rw-rw-rw-   0        0        0     6184 2024-01-08 06:09:44.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.677639 mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/
--rw-rw-rw-   0        0        0     1525 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationBooleanResults.py
--rw-rw-rw-   0        0        0     2205 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationNumberResults.py
--rw-rw-rw-   0        0        0     1741 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationResults.py
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.693076 mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/
--rw-rw-rw-   0        0        0     4496 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/CalculationManagement.py
--rw-rw-rw-   0        0        0     5112 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/ConstantRegion.py
--rw-rw-rw-   0        0        0      762 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.850407 mathematical-expression-py-1.2.1/src/mathematical_expression/exceptional/
--rw-rw-rw-   0        0        0      510 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/exceptional/AbnormalOperation.py
--rw-rw-rw-   0        0        0      443 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/exceptional/ExtractException.py
--rw-rw-rw-   0        0        0      493 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/exceptional/WrongFormat.py
--rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/exceptional/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:05.923317 mathematical-expression-py-1.2.1/src/mathematical_expression/utils/
--rw-rw-rw-   0        0        0     5867 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/utils/NumberUtils.py
--rw-rw-rw-   0        0        0     2795 2024-01-08 06:01:09.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/utils/StrUtils.py
--rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.1/src/mathematical_expression/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 06:57:06.085943 mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/
--rw-rw-rw-   0        0        0    25835 2024-01-08 06:57:05.000000 mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2445 2024-01-08 06:57:05.000000 mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-08 06:57:05.000000 mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-01-08 06:57:05.000000 mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.206839 mathematical-expression-py-1.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    26748 2024-04-03 10:24:33.191262 mathematical-expression-py-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26111 2024-04-03 09:35:27.000000 mathematical-expression-py-1.2.4/README.md
+-rw-rw-rw-   0        0        0      631 2024-04-03 09:44:48.000000 mathematical-expression-py-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 10:24:33.206839 mathematical-expression-py-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.503444 mathematical-expression-py-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.581616 mathematical-expression-py-1.2.4/src/mathematical_expression/
+-rw-rw-rw-   0        0        0     2843 2024-04-03 08:43:37.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.581616 mathematical-expression-py-1.2.4/src/mathematical_expression/core/
+-rw-rw-rw-   0        0        0       51 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.660077 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/
+-rw-rw-rw-   0        0        0     1616 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/Calculation.py
+-rw-rw-rw-   0        0        0      843 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/SharedCalculation.py
+-rw-rw-rw-   0        0        0       45 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.722515 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/__init__.py
+-rw-rw-rw-   0        0        0     3060 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation.py
+-rw-rw-rw-   0        0        0     4326 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.722515 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/
+-rw-rw-rw-   0        0        0     5468 2024-04-03 10:16:14.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/ExpressionFunction.py
+-rw-rw-rw-   0        0        0     1254 2024-04-03 08:33:19.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/Function.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.753762 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/__init__.py
+-rw-rw-rw-   0        0        0     1580 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation.py
+-rw-rw-rw-   0        0        0     4374 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py
+-rw-rw-rw-   0        0        0     4336 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py
+-rw-rw-rw-   0        0        0     2202 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py
+-rw-rw-rw-   0        0        0     6380 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py
+-rw-rw-rw-   0        0        0     6315 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py
+-rw-rw-rw-   0        0        0     8006 2024-04-03 10:23:22.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py
+-rw-rw-rw-   0        0        0     3222 2024-04-03 08:45:17.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/numberCalculation.py
+-rw-rw-rw-   0        0        0     6184 2024-01-08 06:09:44.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.769382 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/
+-rw-rw-rw-   0        0        0     1525 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationBooleanResults.py
+-rw-rw-rw-   0        0        0     2205 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationNumberResults.py
+-rw-rw-rw-   0        0        0     1741 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationResults.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.769382 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/
+-rw-rw-rw-   0        0        0     5177 2024-04-03 08:57:06.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/CalculationManagement.py
+-rw-rw-rw-   0        0        0     5113 2024-04-03 09:44:48.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/ConstantRegion.py
+-rw-rw-rw-   0        0        0      762 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.956866 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/
+-rw-rw-rw-   0        0        0      510 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/AbnormalOperation.py
+-rw-rw-rw-   0        0        0      443 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/ExtractException.py
+-rw-rw-rw-   0        0        0      450 2024-04-03 08:23:31.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/UnsupportedOperationException.py
+-rw-rw-rw-   0        0        0      493 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/WrongFormat.py
+-rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.019359 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/
+-rw-rw-rw-   0        0        0     5867 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/NumberUtils.py
+-rw-rw-rw-   0        0        0     3123 2024-04-03 09:34:50.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/StrUtils.py
+-rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.191262 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/
+-rw-rw-rw-   0        0        0    26748 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2594 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/top_level.txt
```

### Comparing `mathematical-expression-py-1.2.1/LICENSE` & `mathematical-expression-py-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/PKG-INFO` & `mathematical-expression-py-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathematical-expression-py
-Version: 1.2.1
+Version: 1.2.4
 Summary: Python API concise framework for parsing string mathematical expressions
 Author-email: BeardedManZhao <liming7887@qq.com>
 Project-URL: Homepage, https://github.com/BeardedManZhao/mathematical-expression-py
 Project-URL: Bug Tracker, https://github.com/BeardedManZhao/mathematical-expression-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -576,14 +576,42 @@
 
 ```
 计算层数：3
 计算结果：143.0
 计算来源：fastMultiplyOfIntervalsBrackets
 ```
 
+## Advanced Operations
+
+### Registration and use of mathematical function expressions
+
+```python
+import mathematical_expression as me
+
+# 实现一个函数 TODO 这个是数学表达式
+f = "f(x, y) = y + x * x"
+# 开始创建出来函数，并将其注册到管理者中
+me.register_function_expression(f)
+# 将新版函数计算组件获取到
+functionFormulaCalculation2 = me.functionFormulaCalculation2.get_instance("zhao")
+# 启用共享池
+functionFormulaCalculation2.startSharedPool = True
+# 构建需要被计算的数学表达式
+s = "2 * f(1 + 1, 3 - 1)"
+# 检查表达式
+functionFormulaCalculation2.check(s)
+# 计算表达式，并获取结果
+result = functionFormulaCalculation2.calculation(s)
+print(
+    f"计算层数：{result.get_result_layers()}"
+    f"\t计算结果：{result.get_result()}"
+    f"\t计算来源：{result.get_calculation_source_name()}"
+)
+```
+
 <hr>
 
-More information
+## More information
 
 - date: 2022-11-14
 - 切换至 [中文文档](https://github.com/BeardedManZhao/mathematical-expression-py/blob/main/README-Chinese.md)
 - [mathematical-expression-Java](https://github.com/BeardedManZhao/mathematical-expression)
```

### Comparing `mathematical-expression-py-1.2.1/README.md` & `mathematical-expression-py-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -562,14 +562,42 @@
 
 ```
 计算层数：3
 计算结果：143.0
 计算来源：fastMultiplyOfIntervalsBrackets
 ```
 
+## Advanced Operations
+
+### Registration and use of mathematical function expressions
+
+```python
+import mathematical_expression as me
+
+# 实现一个函数 TODO 这个是数学表达式
+f = "f(x, y) = y + x * x"
+# 开始创建出来函数，并将其注册到管理者中
+me.register_function_expression(f)
+# 将新版函数计算组件获取到
+functionFormulaCalculation2 = me.functionFormulaCalculation2.get_instance("zhao")
+# 启用共享池
+functionFormulaCalculation2.startSharedPool = True
+# 构建需要被计算的数学表达式
+s = "2 * f(1 + 1, 3 - 1)"
+# 检查表达式
+functionFormulaCalculation2.check(s)
+# 计算表达式，并获取结果
+result = functionFormulaCalculation2.calculation(s)
+print(
+    f"计算层数：{result.get_result_layers()}"
+    f"\t计算结果：{result.get_result()}"
+    f"\t计算来源：{result.get_calculation_source_name()}"
+)
+```
+
 <hr>
 
-More information
+## More information
 
 - date: 2022-11-14
 - 切换至 [中文文档](https://github.com/BeardedManZhao/mathematical-expression-py/blob/main/README-Chinese.md)
 - [mathematical-expression-Java](https://github.com/BeardedManZhao/mathematical-expression)
```

### Comparing `mathematical-expression-py-1.2.1/pyproject.toml` & `mathematical-expression-py-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "mathematical-expression-py"
-version = "1.2.1"
+version = "1.2.4"
 authors = [
-  { name="BeardedManZhao", email="liming7887@qq.com" },
+    { name = "BeardedManZhao", email = "liming7887@qq.com" },
 ]
 description = "Python API concise framework for parsing string mathematical expressions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/__init__.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,13 +44,21 @@
     """
     注册一个函数到管理者函数库中
     :param fun: 需要被注册的函数实现类对象
     """
     CalculationManagement.register_function(fun)
 
 
+def register_function_expression(fun):
+    """
+    注册一个函数到管理者函数库中
+    :param fun: 需要被注册的函数实现类对象
+    """
+    CalculationManagement.register_function_expression(fun)
+
+
 def unregister_function(fun):
     """
     取消注册一个函数
     :param fun: 需要被取消注册的函数对象
     """
     CalculationManagement.unregister_function(fun)
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/Calculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/Calculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/SharedCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/SharedCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/booleanCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/function/Function.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/Function.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,11 @@
         函数的运行逻辑，需要实现，在该方法中就是函数的主要作用
         :param floats: 函数的形参，这是一个多参函数，函数的实参在这里被传递进来，其中每一个元素都是在表达式中的一个函数形参
         :return: 运算结果，这个函数的返回值是一个多近一出的函数。
         """
         pass
 
     def get_name(self) -> str:
+        """
+        :return: 函数的名字
+        """
         return self.name
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/bracketsCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Time : 2022/11/21 9:52
 # @Author : zhao
 # @Email : liming7887@qq.com
 # @File : functionFormulaCalculation2.py
 # @Project : mathematical-expression-py
-from typing import List
 
 from mathematical_expression.core.calculation.SharedCalculation import SharedCalculation
 from mathematical_expression.core.calculation.number.functionFormulaCalculation import FunctionFormulaCalculation
 from mathematical_expression.core.manager import ConstantRegion, CalculationManagement
 from mathematical_expression.exceptional.ExtractException import ExtractException
 from mathematical_expression.exceptional.WrongFormat import WrongFormat
 from mathematical_expression.utils import NumberUtils
@@ -67,29 +66,31 @@
     count: int = 0
     # 创建函数名称缓冲区
     function_name: list = list()
     # 开始迭代公式中的每一个字符
     for i in range(0, len(string)):
         char = string[i]
         ascii_number: int = ord(char)
-        if ConstantRegion.BA_ASCII <= ascii_number <= ConstantRegion.BZ_ASCII or \
-                ConstantRegion.SZ_ASCII <= ascii_number <= ConstantRegion.SZ_ASCII:
+        if (ConstantRegion.BA_ASCII <= ascii_number <= ConstantRegion.BZ_ASCII) or \
+                (ConstantRegion.SA_ASCII <= ascii_number <= ConstantRegion.SZ_ASCII):
             # 如果是一个字母，代表是函数的名字，这里就切换状态并将名字添加到缓冲区
-            if b:
+            if not b:
                 b = True
-                start.append(i)
+                start.append(i + 1)
             function_name.append(char)
             start.append(start.pop() + 1)
         elif b and char == ConstantRegion.LEFT_BRACKET:
             count += 1
         elif b and char == ConstantRegion.RIGHT_BRACKET:
-            b = False
-            end.append(i)
-            names.append(ConstantRegion.NO_CHAR.join(names))
-            names.clear()
+            count -= 1
+            if count == 0:
+                b = False
+                end.append(i)
+                names.append(ConstantRegion.NO_CHAR.join(function_name))
+                function_name.clear()
 
 
 class FunctionFormulaCalculation2(FunctionFormulaCalculation, SharedCalculation):
     shareStart: list = list()
     shareEnd: list = list()
     shareNames: list = list()
 
@@ -101,22 +102,23 @@
             start = self.shareStart
             end = self.shareEnd
             names = self.shareNames
         else:
             start = list()
             end = list()
             names = list()
+            function_parameter_extraction2(formula, start, end, names)
         while len(start) != 0:
             pop1 = start.pop()
             pop2 = end.pop()
             pop3 = names.pop()
             # 通过函数名字获取到函数
             function = CalculationManagement.get_function_by_name(pop3)
             # 通过索引计算出来函数形参
-            res_list: List[float] = list()
+            res_list: list[float] = list()
             for s in formula[pop1: pop2].split(ConstantRegion.COMMA):
                 res_list.append(super().BRACKETS_CALCULATION_2.calculation(s).get_result())
             formula = formula.replace(formula[pop1 - len(pop3) - 1: pop2 + 1], str(function.run(res_list)))
         return super().BRACKETS_CALCULATION_2.calculation(formula)
 
     def check(self, string: str):
         start = list()
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/numberCalculation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/numberCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationBooleanResults.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationBooleanResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationNumberResults.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationNumberResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/container/CalculationResults.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/CalculationManagement.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/CalculationManagement.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,14 +79,24 @@
         return False
     else:
         logging.info(ConstantRegion.LOG_INFO_register_FUNCTION + name)
         STRING_FUNCTION_HASH_MAP[name] = function
         return True
 
 
+def register_function_expression(function: str):
+    """
+    将一个函数注册到管理者中
+    :param function: 需要注册的函数 对应的数学表达式
+    :return: 注册是否顺利，如果返回True代表注册成功！
+    """
+    from mathematical_expression.core.calculation.function import ExpressionFunction
+    return register_function(ExpressionFunction.parse(function))
+
+
 def unregister_function(function_name: str):
     """
     注销一个函数的注册，通过函数的名字对函数进行注销
     :param function_name: 需要注销的函数的名称
     :return: 注销成功的函数对象
     """
     logging.info(ConstantRegion.LOG_INFO_UNREGISTER_FUNCTION + function_name)
@@ -97,7 +107,16 @@
     """
     注销一个组件的注册，通过组件的名字对组件进行注销
     :param calculation_name: 需要注销的组件名称
     :return: 注销成功的组件
     """
     logging.info(ConstantRegion.LOG_INFO_UNREGISTER_COMPONENT + calculation_name)
     return STRING_CALCULATION_HASH_MAP.pop(calculation_name)
+
+
+def is_function_exist(calculation_name: str):
+    """
+    判断一个函数是否存在
+    :param calculation_name: 需要被判断的函数名字
+    :return: 如果函数存在，返回 true
+    """
+    return calculation_name in STRING_CALCULATION_HASH_MAP
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/ConstantRegion.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/ConstantRegion.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File : ConstantRegion.py
 # @Project : mathematical-expression-py
 # 这里是框架的常量数据池，不建议更改，如果更改了的话，很可能造成运行混乱
 # 如果针对具有固定格式要求的数学公式需要对此处的参数进行配置，请在修改之后进行re_fresh函数的调用
 import logging
 from typing import List
 
-VERSION: float = 1.2
+VERSION: float = 1.24
 STRING_NULL: str = "null"
 LEFT_BRACKET: str = '('
 RIGHT_BRACKET: str = ')'
 DECIMAL_POINT: str = '.'
 EMPTY: str = ' '
 NO_CHAR: str = ''
 COMMA = ','
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/core/manager/__init__.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/utils/NumberUtils.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/utils/NumberUtils.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression/utils/StrUtils.py` & `mathematical-expression-py-1.2.4/src/mathematical_expression/utils/StrUtils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 # @Time : 2022/11/12 15:23
 # @Author : zhao
 # @Email : liming7887@qq.com
 # @File : StrUtils.py
 # @Project : mathematical_expression-py
 from typing import Optional
 
-from mathematical_expression.core.manager import ConstantRegion
 from mathematical_expression.exceptional.AbnormalOperation import AbnormalOperation
 from mathematical_expression.utils import NumberUtils
 
 
 def string_to_double(string: str):
-    """
-    将一个字符串转换成为一个浮点数值
-    :param string: 需要被转换的字符串
-    :return: 转换之后的浮点数值
-    """
-    if len(string) > 0:
-        int_res: int = 0
-        float_res: int = 0
-        int_size = 0
-        float_size = 0
-        is_int: bool = True
-        # 判断是否为负数
-        is_f = string[0] == ConstantRegion.MINUS_SIGN
-        if is_f:
-            string = string[1:]
-        for c in string:
-            if c != ConstantRegion.DECIMAL_POINT and c != ConstantRegion.EMPTY:
-                if is_int:
-                    int_res = NumberUtils.tenfold(int_res) + char_to_integer(c)
-                    int_size += 1
-                else:
-                    float_res = NumberUtils.tenfold(float_res) + char_to_integer(c)
-                    float_size += 1
-            elif c == ConstantRegion.DECIMAL_POINT:
-                if not is_int:
-                    raise AbnormalOperation(f"数值的浮点符号出现次数过多，无法计算{string}")
-                is_int = False
-        res = int_res + float_res / NumberUtils.power_of_ten(10, float_size)
-        return -res if is_f else res
-    else:
-        raise AbnormalOperation("运算出现错误，在进行字符串转数值的时候，字符串的长度为 0，导致错误的发生。")
+    # """
+    # 将一个字符串转换成为一个浮点数值
+    # :param string: 需要被转换的字符串
+    # :return: 转换之后的浮点数值
+    # """
+    # if len(string) > 0:
+    #     int_res: int = 0
+    #     float_res: int = 0
+    #     int_size = 0
+    #     float_size = 0
+    #     is_int: bool = True
+    #     # 判断是否为负数
+    #     is_f = string[0] == ConstantRegion.MINUS_SIGN
+    #     if is_f:
+    #         string = string[1:]
+    #     for c in string:
+    #         if c != ConstantRegion.DECIMAL_POINT and c != ConstantRegion.EMPTY:
+    #             if is_int:
+    #                 int_res = NumberUtils.tenfold(int_res) + char_to_integer(c)
+    #                 int_size += 1
+    #             else:
+    #                 float_res = NumberUtils.tenfold(float_res) + char_to_integer(c)
+    #                 float_size += 1
+    #         elif c == ConstantRegion.DECIMAL_POINT:
+    #             if not is_int:
+    #                 raise AbnormalOperation(f"数值的浮点符号出现次数过多，无法计算{string}")
+    #             is_int = False
+    #     res = int_res + float_res / NumberUtils.power_of_ten(10, float_size)
+    #     return -res if is_f else res
+    # else:
+    #     raise AbnormalOperation("运算出现错误，在进行字符串转数值的时候，字符串的长度为 0，导致错误的发生。")
+    return float(string)
 
 
 def char_to_integer(c: str):
     """
     将一个字符转换成为一个数值
     :param c: 需要被转换的字符
     :return: 转换之后的数值
@@ -60,7 +60,19 @@
                                     "Conversion failed because this is a character that is not a numeric value.\n"
                                     "ERROR => " + c)
     else:
         raise AbnormalOperation("在进行 charToInteger 函数的调用时，您传入的不是一个字符，而是一个字符串，因此发生了错误。\n"
                                 "When calling the charToInteger function, you passed in a string instead of a "
                                 "character, so an error occurred.\n "
                                 "ERROR => " + c)
+
+
+def is_number(c: str):
+    """
+    检查一个字符串是否可以被解析为数值
+    :param c: 需要被检查的字符串
+    :return: 如果可以被解析为数值就返回 True
+    """
+    for c1 in c:
+        if not (48 <= ord(c1) <= 57):
+            return False
+    return True
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/PKG-INFO` & `mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathematical-expression-py
-Version: 1.2.1
+Version: 1.2.4
 Summary: Python API concise framework for parsing string mathematical expressions
 Author-email: BeardedManZhao <liming7887@qq.com>
 Project-URL: Homepage, https://github.com/BeardedManZhao/mathematical-expression-py
 Project-URL: Bug Tracker, https://github.com/BeardedManZhao/mathematical-expression-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -576,14 +576,42 @@
 
 ```
 计算层数：3
 计算结果：143.0
 计算来源：fastMultiplyOfIntervalsBrackets
 ```
 
+## Advanced Operations
+
+### Registration and use of mathematical function expressions
+
+```python
+import mathematical_expression as me
+
+# 实现一个函数 TODO 这个是数学表达式
+f = "f(x, y) = y + x * x"
+# 开始创建出来函数，并将其注册到管理者中
+me.register_function_expression(f)
+# 将新版函数计算组件获取到
+functionFormulaCalculation2 = me.functionFormulaCalculation2.get_instance("zhao")
+# 启用共享池
+functionFormulaCalculation2.startSharedPool = True
+# 构建需要被计算的数学表达式
+s = "2 * f(1 + 1, 3 - 1)"
+# 检查表达式
+functionFormulaCalculation2.check(s)
+# 计算表达式，并获取结果
+result = functionFormulaCalculation2.calculation(s)
+print(
+    f"计算层数：{result.get_result_layers()}"
+    f"\t计算结果：{result.get_result()}"
+    f"\t计算来源：{result.get_calculation_source_name()}"
+)
+```
+
 <hr>
 
-More information
+## More information
 
 - date: 2022-11-14
 - 切换至 [中文文档](https://github.com/BeardedManZhao/mathematical-expression-py/blob/main/README-Chinese.md)
 - [mathematical-expression-Java](https://github.com/BeardedManZhao/mathematical-expression)
```

### Comparing `mathematical-expression-py-1.2.1/src/mathematical_expression_py.egg-info/SOURCES.txt` & `mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/mathematical_expression/core/__init__.py
 src/mathematical_expression/core/calculation/Calculation.py
 src/mathematical_expression/core/calculation/SharedCalculation.py
 src/mathematical_expression/core/calculation/__init__.py
 src/mathematical_expression/core/calculation/bool/__init__.py
 src/mathematical_expression/core/calculation/bool/booleanCalculation.py
 src/mathematical_expression/core/calculation/bool/booleanCalculation2.py
+src/mathematical_expression/core/calculation/function/ExpressionFunction.py
 src/mathematical_expression/core/calculation/function/Function.py
 src/mathematical_expression/core/calculation/function/__init__.py
 src/mathematical_expression/core/calculation/number/__init__.py
 src/mathematical_expression/core/calculation/number/bracketsCalculation.py
 src/mathematical_expression/core/calculation/number/bracketsCalculation2.py
 src/mathematical_expression/core/calculation/number/cumulativeCalculation.py
 src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py
@@ -26,14 +27,15 @@
 src/mathematical_expression/core/container/CalculationResults.py
 src/mathematical_expression/core/container/__init__.py
 src/mathematical_expression/core/manager/CalculationManagement.py
 src/mathematical_expression/core/manager/ConstantRegion.py
 src/mathematical_expression/core/manager/__init__.py
 src/mathematical_expression/exceptional/AbnormalOperation.py
 src/mathematical_expression/exceptional/ExtractException.py
+src/mathematical_expression/exceptional/UnsupportedOperationException.py
 src/mathematical_expression/exceptional/WrongFormat.py
 src/mathematical_expression/exceptional/__init__.py
 src/mathematical_expression/utils/NumberUtils.py
 src/mathematical_expression/utils/StrUtils.py
 src/mathematical_expression/utils/__init__.py
 src/mathematical_expression_py.egg-info/PKG-INFO
 src/mathematical_expression_py.egg-info/SOURCES.txt
```

