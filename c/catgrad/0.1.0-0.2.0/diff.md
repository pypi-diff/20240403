# Comparing `tmp/catgrad-0.1.0.tar.gz` & `tmp/catgrad-0.2.0.tar.gz`

## Comparing `catgrad-0.1.0.tar` & `catgrad-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/combinators.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/compile.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/functor.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/layers.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/operations.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/parameters.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/rdops.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/target/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/target/ast.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/target/python/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/target/python/array_backend.py
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 catgrad-0.1.0/catgrad/target/python/codegen.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 catgrad-0.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 catgrad-0.1.0/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 catgrad-0.1.0/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 catgrad-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 catgrad-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/combinators.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/compile.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/layers.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/signature.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/bidirectional/functor.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/bidirectional/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/core/__init__.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/core/operation.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/special/definition.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/special/parameter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/ast.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/special.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/__init__.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/numpy.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/torch.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/type.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/__init__.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/codegen.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/definition.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/operation.py
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 catgrad-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 catgrad-0.2.0/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 catgrad-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 catgrad-0.2.0/PKG-INFO
```

### Comparing `catgrad-0.1.0/catgrad/combinators.py` & `catgrad-0.2.0/catgrad/combinators.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.1.0/catgrad/functor.py` & `catgrad-0.2.0/catgrad/bidirectional/functor.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Translate RDOps to basic array operations
 class Forget(FrobeniusFunctor):
     def map_objects(self, objects: FiniteFunction) -> IndexedCoproduct:
         return self.IndexedCoproduct().elements(objects)
 
     def map_operations(self, x: FiniteFunction, sources: IndexedCoproduct, targets: IndexedCoproduct) -> OpenHypergraph:
         # we lose a lot of speed here using tensor_list, but it's simpler code
-        fs = [ x.arrow() for x in x.table ]
+        fs = [ x.to_core() for x in x.table ]
         return self.OpenHypergraph().tensor_list(fs, sigma_0, sigma_1)
 
 # Map rdops to their fwd maps
 class Fwd(FrobeniusFunctor):
     def map_objects(self, objects: FiniteFunction) -> IndexedCoproduct:
         return self.IndexedCoproduct().elements(objects)
 
@@ -33,8 +33,12 @@
 
 # Map arrows into their 'bidirectional' form consisting of both fwd and rev passes in opposite directions
 class Bidirectional(Optic):
     F = Fwd()
     R = Rev()
 
     def residual(self, x: FiniteFunction, A: IndexedCoproduct, B: IndexedCoproduct) -> IndexedCoproduct:
-        return IndexedCoproduct.from_list(None, [op.residual() for op in x], dtype=object)
+        # NOTE: we don't need the types of operations to calculate the residual
+        return residual(x)
+
+def residual(x: FiniteFunction):
+    return IndexedCoproduct.from_list(None, [op.residual() for op in x], dtype=object)
```

### Comparing `catgrad-0.1.0/catgrad/layers.py` & `catgrad-0.2.0/catgrad/layers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """ neural network layers """
 from catgrad.signature import NdArrayType
 from catgrad.combinators import canonical
-from catgrad.rdops import *
-from catgrad.parameters import parameter
+from catgrad.bidirectional.operation import *
+from catgrad.special.parameter import parameter
 
+def flatten(X: NdArrayType, Y: NdArrayType):
+    return op(Reshape(X, Y))
+
+# linear is OK when you have a *batch* of A inputs of type (1 → B) and you want to multiply them all by the same matrix
+# (B ⇒ C) to get a batch of A outputs (A ⇒ C).
+# If you need to "pointwise batch", use "batch_linear"
 def linear(A: NdArrayType, B: NdArrayType, C: NdArrayType):
     if not (A.dtype == B.dtype and B.dtype == C.dtype):
-        raise ValueError("linear: dtypes must be equal, but got dtypes {A.dtype=} {B.dtype=} {C.dtype=}")
+        raise ValueError(f"linear: dtypes must be equal, but got dtypes {A.dtype=} {B.dtype=} {C.dtype=}")
     return (identity(obj(A+B)) @ parameter(obj(B+C))) >> op(Compose(A,B,C))
 
 def bias(A: NdArrayType):
     return (parameter(obj(A)) @ identity(obj(A))) >> add(obj(A))
 
 sigmoid = canonical(lambda T: op(Sigmoid(T)))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `catgrad-0.1.0/catgrad/operations.py` & `catgrad-0.2.0/catgrad/core/operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,49 +21,94 @@
     def source(self): return obj(self.T)
     def target(self): return obj(self.T, self.T)
 
 @dataclass
 class NCopy:
     # TODO: introduce split/join and mention naturality of Broadcast w.r.t. them.
     """ NCopy is like Copy, but on tensor dimensions.
-    ``NCopy(N,A) : A → N+A`` is like the N-fold copy of a tensor of shape A, then packed into a tensor.
+    ``NCopy(N,T) : N → N+T`` is like the T-fold copy of a tensor of shape N, then packed into a tensor.
     """
     N: NdArrayType
     T: NdArrayType
-    def source(self): return obj(self.T)
+    def source(self): return obj(self.N)
     def target(self): return obj(self.N + self.T)
 
 @dataclass
 class Discard:
     T: NdArrayType
     def source(self): return obj(self.T)
     def target(self): return obj()
 
 @dataclass
+class NSplit:
+    """ ``NSplit(T, k) : T*k → T●T..k...T`` splits a tensor into individual outputs """
+    T: NdArrayType
+    k: int
+    def __post_init__(self):
+        # TODO: this should really be equivalent to discarding.
+        assert self.k > 0, "cannot split into fewer than 1 outputs"
+
+    def source(self):
+        N = NdArrayType((self.k,), self.T.dtype)
+        return obj(self.T + N)
+    def target(self): return obj(*([self.T]*self.k)) # N●..k..●N
+
+@dataclass
+class NConcatenate:
+    """ ``NConcatenate(N, k) : N●N..k...N → N*k`` concatenates k tensors into a single outputs """
+    T: NdArrayType
+    k: int
+    def source(self): return obj(*([self.T]*self.k)) # N●..k..●N
+    def target(self):
+        N = NdArrayType((self.k,), self.T.dtype)
+        return obj(self.T + N)
+
+@dataclass
 class Add:
     T: NdArrayType
     def source(self): return obj(self.T, self.T)
     def target(self): return obj(self.T)
 
 @dataclass
 class NAdd:
-    """ ``NAdd(N, T)`` sums a tensor of type N + T over the N dimensions. """
+    """ ``NAdd(N, T) : N×T → N`` sums a tensor of type N + T over the T dimensions. """
     N: NdArrayType
     T: NdArrayType
     def source(self): return obj(self.N + self.T)
-    def target(self): return obj(self.T)
+    def target(self): return obj(self.N)
+
+@dataclass
+class NMax:
+    """ ``NMax(N, T) : N×T → N`` returns the maximum of a tensor of type N + T over the T dimensions. """
+    N: NdArrayType
+    T: NdArrayType
+    def __post_init__(self):
+        if prod(self.N.shape + self.T.shape) <= 0:
+            raise ValueError(f"Cannot NMax zero-element vector: {self}")
+
+    def source(self): return obj(self.N + self.T)
+    def target(self): return obj(self.N)
 
 @dataclass
 class Negate:
     """ ``Negate(T) : T×T → T`` computes ``-x``. """
     T: NdArrayType
     def source(self): return obj(self.T)
     def target(self): return obj(self.T)
 
 @dataclass
+class Invert:
+    T: NdArrayType
+    def __post_init__(self):
+        if self.T.dtype.is_floating():
+            raise ValueError("Invert operation not supported for floating dtypes")
+    def source(self): return obj(self.T)
+    def target(self): return obj(self.T)
+
+@dataclass
 class Subtract:
     """ ``Sub(T) : T×T → T`` computes ``(x - y)`` """
     T: NdArrayType
     def source(self): return obj(self.T, self.T)
     def target(self): return obj(self.T)
 
 scalar = int | float
@@ -71,16 +116,14 @@
 class Constant:
     T: NdArrayType
     x: scalar # will be cast to T.dtype
 
     def __post_init__(self):
         if not isinstance(self.x, scalar):
             raise ValueError(f"constant {self.x} is not a scalar {scalar}")
-        if self.T.shape != ():
-            raise ValueError(f"Constant.T.shape must be () but was {self.T.shape}")
 
     def source(self): return obj()
     def target(self): return obj(self.T)
 
 ################################################################################
 # Isomorphisms
 
@@ -121,14 +164,23 @@
 @dataclass
 class Multiply:
     T: NdArrayType
     def source(self): return obj(self.T, self.T)
     def target(self): return obj(self.T)
 
 ################################################################################
+# Comparators
+
+@dataclass
+class Gt:
+    T: NdArrayType
+    def source(self): return obj(self.T, self.T)
+    def target(self): return obj(self.T)
+
+################################################################################
 # Partial functions arithmetic
 
 @dataclass
 class Divide:
     """ `Divide: T × T → T` is the partial function `<x,y> → x/y`. """
     T: NdArrayType
     def source(self): return obj(self.T, self.T)
@@ -140,22 +192,35 @@
     T: NdArrayType
     def source(self): return obj(self.T, self.T)
     def target(self): return obj(self.T)
 
 # TODO: tidy this up
 # helper for the 'exp' circuit.
 def exp1(T: NdArrayType):
-    U = NdArrayType((), T.dtype)
-    a = op(Constant(U, math.e))
-    b = op(NCopy(T, U))
-    return ((a >> b) @ identity(obj(T))) >> op(Power(T))
+    return (op(Constant(T, math.e)) @ identity(obj(T))) >> op(Power(T))
 
 ################################################################################
-# Matrix multiplication
+# Matrix multiplication and tensor composition
+
+@dataclass
+class MatrixMultiply:
+    """ Batched matrix multiplication """
+    N: NdArrayType
+    A: NdArrayType
+    B: NdArrayType
+    C: NdArrayType
+    def __post_init__(self):
+        # N can be any type, but A, B, C must be a single dimension
+        for t in [self.A, self.B, self.C]:
+            assert len(t.shape) == 1
+
+    def source(self): return obj(self.N+self.A+self.B, self.N+self.B+self.C)
+    def target(self): return obj(self.N+self.A+self.C)
 
+# TODO: should we get rid of this?
 @dataclass
 class Compose:
     """ Composition of tensors ``f : A → B`` and ``g : B → C`` along ``B``, so
     that ``Compose(f, g) : A → C``
     """
     A: NdArrayType
     B: NdArrayType
@@ -163,8 +228,8 @@
 
     def source(self): return obj(self.A+self.B, self.B+self.C)
     def target(self): return obj(self.A+self.C)
 
 ################################################################################
 # All the array operations in a union type
 
-operation = Copy | NCopy | Discard | Add | NAdd | Constant | Reshape | Permute | Multiply | Compose
+operation = Copy | NCopy | NSplit | NConcatenate | Discard | Add | NAdd | Constant | Reshape | Permute | Multiply | MatrixMultiply | Compose
```

### Comparing `catgrad-0.1.0/catgrad/parameters.py` & `catgrad-0.2.0/catgrad/special/parameter.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.1.0/catgrad/rdops.py` & `catgrad-0.2.0/catgrad/bidirectional/operation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import numpy as np
 from dataclasses import dataclass
 from abc import abstractmethod
 from open_hypergraphs import OpenHypergraph, FiniteFunction, IndexedCoproduct, FrobeniusFunctor
 
 from catgrad.signature import NdArrayType, obj, op, sigma_0, sigma_1
-import catgrad.operations as ops
+import catgrad.core.operation as ops
+from catgrad.special.definition import Definition
 from catgrad.combinators import *
 
 class Optic:
     @abstractmethod
     def source(self) -> FiniteFunction:
         ...
 
     @abstractmethod
     def target(self) -> FiniteFunction:
         ...
 
     # Map this Optic into its underlying array operations
     # e.g., Sigmoid will map to exp / (1 + exp)
     @abstractmethod
-    def arrow(self) -> OpenHypergraph:
+    def to_core(self) -> OpenHypergraph:
         ...
 
     # Optic structure
     @abstractmethod
     def fwd(self) -> OpenHypergraph:
         ...
 
@@ -62,181 +63,293 @@
     def residual(self) -> FiniteFunction:
         return obj()
 
 ################################################################################
 # basic operations as optics
 
 class Copy(ops.Copy, Dagger):
-    def arrow(self): return op(ops.Copy(self.T))
+    def to_core(self): return op(ops.Copy(self.T))
     def dagger(self): return op(Add(self.T))
 
 class NCopy(ops.NCopy, Dagger):
-    def arrow(self): return op(ops.NCopy(self.N, self.T))
+    def to_core(self): return op(ops.NCopy(self.N, self.T))
     def dagger(self): return op(NAdd(self.N, self.T))
 
 class Discard(ops.Discard, Dagger):
-    def arrow(self): return op(ops.Discard(self.T))
-    # NOTE: we do one scalar zero and broadcast into the correct shape
+    def to_core(self): return op(ops.Discard(self.T))
     def dagger(self):
-        U = NdArrayType((), self.T.dtype)
-        return op(Constant(U, 0)) >> op(NCopy(self.T, U))
+        return op(Constant(self.T, 0))
+
+class NSplit(ops.NSplit, Dagger):
+    def to_core(self): return op(ops.NSplit(self.T, self.k))
+    def dagger(self): return op(NConcatenate(self.T, self.k))
+
+class NConcatenate(ops.NConcatenate, Dagger):
+    def to_core(self): return op(ops.NConcatenate(self.T, self.k))
+    def dagger(self): return op(NSplit(self.T, self.k))
 
 class Add(ops.Add, Dagger):
-    def arrow(self): return op(ops.Add(self.T))
+    def to_core(self): return op(ops.Add(self.T))
     def dagger(self): return op(Copy(self.T))
 
 class NAdd(ops.NAdd, Dagger):
-    def arrow(self): return op(ops.NAdd(self.N, self.T))
+    def to_core(self): return op(ops.NAdd(self.N, self.T))
     def dagger(self): return op(NCopy(self.N, self.T))
 
 class Subtract(ops.Add, Dagger):
-    def arrow(self): return op(ops.Subtract(self.T))
+    def to_core(self): return op(ops.Subtract(self.T))
     def dagger(self):
         T = obj(self.T)
         return copy(T) >> (identity(T) @ negate(T))
 
 class Negate(ops.Negate, Dagger):
-    def arrow(self): return op(ops.Negate(self.T))
+    def to_core(self): return op(ops.Negate(self.T))
+    def dagger(self): return op(self)
+
+class Invert(ops.Invert, Dagger):
+    def to_core(self): return op(ops.Invert(self.T))
     def dagger(self): return op(self)
 
 class Constant(ops.Constant, Dagger):
-    def arrow(self): return op(ops.Constant(self.T, self.x))
+    def to_core(self): return op(ops.Constant(self.T, self.x))
     def dagger(self): return op(Discard(self.T))
 
 class Reshape(ops.Reshape, Dagger):
-    def arrow(self): return op(ops.Reshape(self.X, self.Y))
+    def to_core(self): return op(ops.Reshape(self.X, self.Y))
     def dagger(self): return op(Reshape(self.Y, self.X))
 
 class Permute(ops.Permute, Dagger):
-    def arrow(self): return op(ops.Permute(self.T, self.p))
-    def dagger(self): return op(Permute(self.T, np.argsort(self.p).tolist()))
+    def to_core(self): return op(ops.Permute(self.T, self.p))
+    def dagger(self): return op(Permute(self.target()(0), np.argsort(self.p).tolist()))
+
+class Gt(ops.Gt, Optic):
+    def to_core(self): return op(ops.Gt(self.T))
+    def residual(self): return obj()
+    def fwd(self): return op(self)
+    def rev(self):
+        return op(Discard(self.T)) >> zero(obj(self.T, self.T))
 
 class Multiply(ops.Multiply, Lens):
-    def arrow(self): return op(ops.Multiply(self.T))
+    def to_core(self): return op(ops.Multiply(self.T))
     def rev(self):
         T = obj(self.T)
         mul = op(self)
         lhs = (twist(T, T) @ copy(T))
         mid = (identity(T) @ twist(T, T) @ identity(T))
         rhs = mul @ mul
         return lhs >> mid >> rhs
 
+# Scale by the reciprocal of a scalar. Maps to division, but it's a Dagger
+@dataclass
+class ScaleInverse(Dagger):
+    T: NdArrayType
+    s: ops.scalar
+
+    def __post_init__(self): assert self.s != 0
+    def source(self): return obj(self.T)
+    def target(self): return obj(self.T)
+
+    def to_core(self):
+        return (identity(obj(self.T)) @ op(ops.Constant(self.T, self.s))) >> op(ops.Divide(self.T))
+    def dagger(self):
+        return op(self)
+
+@dataclass
+class Exponentiate(Lens):
+    T: NdArrayType
+    s: ops.scalar
+
+    def __post_init__(self):
+        if not self.T.dtype.is_floating():
+            raise ValueError("Exponentiate is not defined for non-floating-point dtypes")
+
+    def source(self): return obj(self.T)
+    def target(self): return obj(self.T)
+
+    def to_core(self):
+        return (identity(obj(self.T)) @ op(ops.Constant(self.T, self.s))) >> op(ops.Power(self.T))
+    def rev(self):
+        X = obj(self.T)
+
+        #       <s|----\
+        #               ○---
+        # --[^(s-1)]---/
+        diff = op(Exponentiate(self.T, self.s-1)) >> scale(self.s)(X)
+
+        # --[diff]--\
+        #            ○---
+        # ----------/
+        rev = (diff @ identity(X)) >> multiply(X)
+
+        return rev
+
+class MatrixMultiply(ops.MatrixMultiply, Lens):
+    """ Tensor composition (diagrammatic order) """
+    def to_core(self): return op(ops.MatrixMultiply(self.N, self.A, self.B, self.C))
+    def rev(self):
+        N, A, B, C = self.N, self.A, self.B, self.C
+        n = len(self.N.shape)
+        # all the indices in the batch N stay the same; final two swap.
+        ixs = list(range(n)) + [n+1, n]
+
+        lhs = op(Permute(N+A+B, ixs)) @ op(Permute(N+B+C, ixs)) @ copy(obj(N+A+C))
+        p = permutation(lhs.target, [2, 1, 0, 3])
+        rhs = op(MatrixMultiply(N, A, C, B)) @ op(MatrixMultiply(N, B, A, C))
+        return lhs >> p >> rhs
+
+
 class Compose(ops.Compose, Lens):
-    def arrow(self): return op(ops.Compose(self.A, self.B, self.C))
+    """ Tensor composition (diagrammatic order) """
+    def to_core(self): return op(ops.Compose(self.A, self.B, self.C))
     def rev(self):
         A, B, C = self.A, self.B, self.C
         t_AB = FiniteFunction.twist(len(B.shape), len(A.shape)).table.tolist()
         t_BC = FiniteFunction.twist(len(C.shape), len(B.shape)).table.tolist()
 
         lhs = op(Permute(A+B, t_AB)) @ op(Permute(B+C, t_BC)) @ copy(obj(A + C))
         p = permutation(lhs.target, [2, 1, 0, 3])
         rhs = op(Compose(A, C, B)) @ op(Compose(B, A, C))
         return lhs >> p >> rhs
 
 ################################################################################
 # Canonical combinators
 
-def full1(c: ops.scalar):
-    """ ``full1(c)`` returns a function f(T: NdArrayType) which constructs a
-    circuit of type ``I → T`` representing the constant array of type T filled
-    with values ``c``. """
-    def full1_wrapped(T: NdArrayType):
-        U = NdArrayType((), T.dtype)
-        a = op(Constant(U, c))
-        b = op(NCopy(T, U))
-        return a >> b
-    return full1_wrapped
-
 copy = canonical(lambda T: op(Copy(T)))
 discard = canonical(lambda T: op(Discard(T)))
 
 add  = canonical(lambda T: op(Add(T)))
-zero = canonical(full1(0))
+zero = canonical(lambda T: op(Constant(T, 0)))
 subtract = canonical(lambda T: op(Subtract(T)))
 negate = canonical(lambda T: op(Negate(T)))
 
 multiply = canonical(lambda T: op(Multiply(T)))
+
 # could also call this "full".
-constant = lambda c: canonical(full1(c))
+def constant(c):
+    return canonical(lambda T: op(Constant(T, c)))
+
+def increment(c):
+    """ increment by a constant """
+    def increment_wrapper(A: FiniteFunction):
+        return (constant(c)(A) @ identity(A)) >> add(A)
+    return increment_wrapper
 
-# multiply by a constant
 def scale(c):
+    """ multiply by a constant """
     def scale_wrapper(A: FiniteFunction):
         return (constant(c)(A) @ identity(A)) >> multiply(A)
     return scale_wrapper
 
-################################################################################
-
-# Translate RDOps to basic array operations
-class Forget(FrobeniusFunctor):
-    def map_objects(self, objects: FiniteFunction) -> IndexedCoproduct:
-        return self.IndexedCoproduct().elements(objects)
-
-    def map_operations(self, x: FiniteFunction, sources: IndexedCoproduct, targets: IndexedCoproduct) -> OpenHypergraph:
-        # we lose a lot of speed here using tensor_list, but it's simpler code
-        fs = [ x.arrow() for x in x.table ]
-        return self.OpenHypergraph().tensor_list(fs, sigma_0, sigma_1)
+def scale_inverse(s):
+    """ divide by a constant """
+    scale_inverse_wrapper = canonical(lambda T: op(ScaleInverse(T, s)))
+    return scale_inverse_wrapper
+
+def exponentiate(s):
+    """ exponentiate by a constant ``x^s`` """
+    exponentiate_wrapper = canonical(lambda T: op(Exponentiate(T, s)))
+    return exponentiate_wrapper
+
+
+########################################
+# comparators
+
+gt = canonical(lambda T: op(Gt(T)))
+
+def gt_constant(c):
+    def gt_constant_wrapper(A: FiniteFunction):
+        return (identity(A) @ constant(c)(A)) >> gt(A)
+    return gt_constant_wrapper
 
 ################################################################################
 # Other definitions
 
-@dataclass
-class Sigmoid(Lens):
+@dataclass(frozen=True)
+class Sigmoid(Definition, Lens):
     T: NdArrayType
     def source(self): return obj(self.T)
     def target(self): return obj(self.T)
 
     def __post_init__(self):
         if not self.T.dtype.is_floating():
             raise ValueError("Sigmoid is not defined for non-floating-point dtypes")
 
-    # TODO: tidy me
+    ########################################
+    # Sigmoid as a Core definition
+
+    # The definition of the Sigmoid function in terms of Core ops
     def arrow(self):
-        # x → exp(x) / (1 + exp(x))
-        # x → 1 / (1 + exp(-x))
+        # here we write a morphism in *core*!
         T = self.T
         U = NdArrayType((), T.dtype)
 
-        # the 1 constant at shape T
-        full1 = op(ops.Constant(U, 1)) >> op(ops.NCopy(T, U))
+        full1 = op(ops.Constant(T, 1))
+
+        # inc(x) := 1 + x
         inc = (full1 @ identity(obj(T))) >> op(ops.Add(T))
 
+        # den(x) := 1 + exp(-x)
         den = op(ops.Negate(T)) >> ops.exp1(T) >> inc
+
+        #      1
+        # -----------
+        # 1 + exp(-x)
         return (full1 @ den) >> op(ops.Divide(T))
 
+    ########################################
+    # Sigmoid as an Optic
+
+    # we want this to appear as a Definition in core, so we just return the op
+    # as a singleton diagram.
+    def to_core(self):
+        return op(self)
+
+    # The forward map is like Lens, but we copy the *output*, not the input.
+    def fwd(self):
+        return op(self) >> copy(self.source())
+
+    # The reverse map is σ(x) · (1 - σ(x)) · dy
     def rev(self):
-        # TODO: implement arithmetic operations on arrows so we can write
         # σ * (1 - σ) * dy
+        #
+        #         /----------\
+        # σ(x) --●            *---\
+        #         \-- (1-) --/     *---
+        #                         /
+        # dy   ------------------/
         T = obj(self.T)
-        σ = op(self)
-        f = (constant(1)(T) @ σ) >> subtract(T) # 1 - σ
-        grad = copy(T) >> (σ @ f) >> multiply(T) # σ * (1 - σ)
+        id_T = identity(T)
+        dec_1 = (constant(1)(T) @ id_T) >> subtract(T) # 1 - x
+        grad = copy(T) >> (id_T @ dec_1) >> multiply(T) # σ * (1 - σ)
         return (grad @ identity(T)) >> multiply(T) # σ * (1 - σ) * dy
 
 sigmoid = canonical(lambda T: op(Sigmoid(T)))
 
+def relu(X):
+    return copy(X) >> (gt_constant(0)(X) @ identity(X)) >> multiply(X)
+
 ################################################################################
 # Learner lenses
 
 @dataclass
 class SGD(Lens):
     T: NdArrayType
     c: ops.scalar
     def source(self): return obj(self.T)
     def target(self): return obj(self.T)
-    def arrow(self): return identity(obj(self.T))
+    def to_core(self): return identity(obj(self.T))
     def rev(self):
         T = obj(self.T)
         return (identity(T) @ scale(self.c)(T)) >> subtract(T)
 
 def sgd(c: ops.scalar):
     return canonical(lambda T: op(SGD(T, c)))
 
 @dataclass
 class MSE(Lens):
     T: NdArrayType
     def source(self): return obj(self.T)
     def target(self): return obj(self.T)
-    def arrow(self): return identity(obj(self.T))
+    def to_core(self): return identity(obj(self.T))
     def rev(self): return subtract(obj(self.T))
 
 mse = canonical(lambda T: op(MSE(T)))
```

### Comparing `catgrad-0.1.0/catgrad/signature.py` & `catgrad-0.2.0/catgrad/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,32 @@
 
 Shape = Tuple
 
 class Dtype(Enum):
     """ Dtypes correspond to semirings: a choice of dtype specifies field/(semi)ring operations. """
     int32 = auto()
     float32 = auto()
+    bool = auto()
 
     def is_floating(self):
         return self.value in _FLOATING_DTYPES
 _FLOATING_DTYPES = { Dtype.float32.value }
 
-@dataclass
+@dataclass(frozen=True)
 class NdArrayType:
     """ An NdArrayType is the *metadata* for an N-dimensional array.
     It consists of a shape and a dtype, but not data.
     The values of type ``NdArrayType`` are the generating objects of our category.
     """
     shape: Shape
     dtype: Dtype
 
+    def __post_init__(self):
+        assert type(self.shape) is tuple, "NdArrayType.shape must be a tuple"
+
     @classmethod
     def from_ndarray(cls, x: np.ndarray):
         """ Create an ``NdArrayType`` from an object with shape and dtype """
         return NdArrayType(x.shape, x.dtype)
 
     # coproduct of shapes for convenience!
     # TODO: should this be __mul__? It's the cartesian product!
```

### Comparing `catgrad-0.1.0/catgrad/target/ast.py` & `catgrad-0.2.0/catgrad/target/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import numpy as np
 from typing import List
 from dataclasses import dataclass
 
 from open_hypergraphs import FiniteFunction, OpenHypergraph
 from open_hypergraphs.numpy import layer
-from catgrad.operations import operation
+from catgrad.core.operation import operation
 
 # An `Apply` represents the application of some operation to arguments lhs and rhs.
 @dataclass
 class Apply:
     """ The application of an operation of a given type to some arguments (lhs)
     producing some return values (lhs) """
     op: operation # the operation itself
```

### Comparing `catgrad-0.1.0/catgrad/target/python/array_backend.py` & `catgrad-0.2.0/catgrad/target/python/array_backend/type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from typing import Protocol, TypeVar, Type, Any, List, Tuple
-import numpy as np
-
 from catgrad import signature
 
 # Generic NdArray type, supporting pointwise arithmetic and matmul.
 class NdArray(Protocol):
     shape: Tuple
     dtype: Any
 
@@ -23,69 +21,48 @@
     def __matmul__(self, other):
         ...
 
 A = TypeVar('A', bound=NdArray)
 
 class ArrayBackend(Protocol[A]):
     """ An ArrayBackend is an implementation of the basic array operations in
-    :py:mod:`catgrad.operations`.
+    :py:mod:`catgrad.core.operation`.
     See for example the :py:class:`Numpy` backend. """
     @staticmethod
     def dtype(d: signature.Dtype) -> Any:
         ...
 
     @staticmethod
-    def constant(x: Any) -> A:
+    def constant(x: Any, shape: Tuple, dtype: signature.Dtype) -> A:
         ...
 
     @staticmethod
     def ncopy(shape: Tuple, x: A) -> A:
         ...
 
     @staticmethod
-    def nadd(shape: Tuple, x: A) -> A:
+    def nsplit(x: A, k: int) -> List[A]:
         ...
 
     @staticmethod
-    def reshape(x: A, shape: Tuple) -> A:
+    def nconcatenate(xs: List[A], k: int) -> List[A]:
         ...
 
     @staticmethod
-    def permute(x: A, p: List[int]):
+    def nadd(dims: Tuple, x: A) -> A:
         ...
 
     @staticmethod
-    def compose(x: A, y: A, axes: int) -> A:
+    def nmax(dims: Tuple, x: A) -> A:
         ...
 
-# A Numpy array backend
-class Numpy:
-    @staticmethod
-    def dtype(d: signature.Dtype) -> Any:
-        match d:
-            case signature.Dtype.int32: return np.int32
-            case signature.Dtype.float32: return np.float32
-            case x: raise ValueError(f"dtype {x} is not implemented for Numpy")
-
     @staticmethod
-    def constant(x: Any, dtype: signature.Dtype) -> np.ndarray:
-        return np.array(x, dtype=Numpy.dtype(dtype))
-
-    @staticmethod
-    def ncopy(shape: Tuple, x: np.ndarray) -> np.ndarray:
-        return np.broadcast_to(x, (*shape, *x.shape))
-
-    @staticmethod
-    def nadd(shape: Tuple, x: np.ndarray) -> np.ndarray:
-        return x.sum(tuple(range(len(shape))))
-
-    @staticmethod
-    def reshape(x: np.ndarray, shape: Tuple) -> np.ndarray:
-        return np.reshape(x, shape)
+    def reshape(x: A, shape: Tuple) -> A:
+        ...
 
     @staticmethod
-    def permute(x: np.ndarray, p: List[int]):
-        return np.transpose(x, p)
+    def permute(x: A, p: List[int]):
+        ...
 
     @staticmethod
-    def compose(x: np.ndarray, y: np.ndarray, axes: int) -> np.ndarray:
-        return np.tensordot(x, y, axes=axes)
+    def compose(x: A, y: A, axes: int) -> A:
+        ...
```

### Comparing `catgrad-0.1.0/catgrad/target/python/codegen.py` & `catgrad-0.2.0/catgrad/target/python/codegen/operation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+""" Generate python expressions for each operation in catgrad.core.operation """
 import ast
-from typing import Type, Any, List, Tuple, Callable
+from typing import Type, List, Tuple, Callable
 
-from catgrad.signature import Dtype, NdArrayType, obj
-import catgrad.operations as ops
+from catgrad.signature import Dtype
+import catgrad.core.operation as ops
 from catgrad.target.ast import *
-from catgrad.target.python.array_backend import Numpy
 
 ################################################################################
 # Helpers
 
 def _assert_identifier(name: str):
     if not name.isidentifier():
         raise ValueError(f"name {name} is not a valid identifier")
@@ -18,46 +18,59 @@
 
 def load(i: int):
     return ast.Name(name_id(i), ctx=ast.Load())
 
 def store(i: int):
     return ast.Name(name_id(i), ctx=ast.Store())
 
+def expr_lhs(apply: Apply):
+    """ Return the LHS (targets) of an assignment as an AST.
+    For example, when ``apply`` has lhs [x0, x1, x2], this will return a tuple
+    (x0, x1, x2) with context Store.
+    """
+    if len(apply.lhs) == 0:
+        return []
+    elif len(apply.lhs) == 1:
+        lhs = store(apply.lhs[0])
+    else:
+        lhs = ast.Tuple(elts=[ store(i) for i in apply.lhs ], ctx=ast.Store())
+    return lhs
+
 def expr(fn: Callable[[Apply, List[ast.Name]], ast.expr]) -> Callable[[Apply], List[ast.Assign]]:
     """ A decorator to turn a function of type
     ``Apply → ast.expr``
     into one of type
     ``Apply → List[ast.Assign]``
     """
     def expr_wrapper(apply: Apply):
-        if len(apply.lhs) == 0:
-            return []
-        elif len(apply.lhs) == 1:
-            lhs = store(apply.lhs[0])
-        else:
-            lhs = ast.Tuple(elts=[ store(i) for i in apply.lhs ], ctx=ast.Store())
-
+        lhs = expr_lhs(apply)
         args = [ load(i) for i in apply.rhs ]
         expr = fn(apply, args)
         return [ast.Assign(targets=[lhs], value=expr)]
 
     return expr_wrapper
 
 def binop(b) -> Callable[[Apply], List[ast.Assign]]:
     def binop_wrapper(a: Apply, args: List[ast.Name]) -> ast.expr:
         assert len(args) == 2
         return ast.BinOp(left=args[0], op=b, right=args[1])
     return expr(binop_wrapper)
 
+def comparison(b) -> Callable[[Apply], List[ast.Assign]]:
+    def binop_wrapper(a: Apply, args: List[ast.Name]) -> ast.expr:
+        assert len(args) == 2
+        return ast.Compare(left=args[0], ops=[b], comparators=[args[1]])
+    return expr(binop_wrapper)
+
 def _call_backend(method: str, args) -> ast.Call:
     # AST expression for calling a backend method, e.g., "self.backend.compose(x, y, z)"
     _assert_identifier(method)
     return ast.Call(
         func=ast.Attribute(
-            value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='backend', ctx=ast.Load()),
+            value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='_backend', ctx=ast.Load()),
             attr=method, ctx=ast.Load()),
         args=args, keywords=[])
 
 ################################################################################
 # Expression handlers: functions turning operations into python ast.expr nodes.
 
 @expr
@@ -72,44 +85,77 @@
     # Discarding produces no assignment statements.
     return []
 
 @expr
 def ncopy(a: Apply, args: List[ast.Name]) -> ast.expr:
     assert type(a.op) == ops.NCopy
     assert len(args) == 1
-    return _call_backend('ncopy', [ast.Constant(value=a.op.N.shape), args[0]])
+    return _call_backend('ncopy', [ast.Constant(value=a.op.T.shape), args[0]])
+
+@expr
+def nsplit(a: Apply, args: List[ast.Name]) -> ast.expr:
+    assert type(a.op) == ops.NSplit
+    assert len(args) == 1
+    return _call_backend('nsplit', [args[0], ast.Constant(value=a.op.k)])
+
+@expr
+def nconcatenate(a: Apply, args: List[ast.Name]) -> ast.expr:
+    # variadic; should have k arguments
+    assert type(a.op) == ops.NConcatenate
+    assert len(args) == a.op.k
+    var_args = ast.List(elts=args, ctx=ast.Load())
+    return _call_backend('nconcatenate', [var_args, ast.Constant(value=a.op.k)])
 
 @expr
 def nadd(a: Apply, args: List[ast.Name]) -> ast.expr:
     assert type(a.op) == ops.NAdd
     assert len(args) == 1
-    return _call_backend('nadd', [ast.Constant(value=a.op.N.shape), args[0]])
+    # dimensions should be e.g., (-3, -2, -1) for
+    dims = tuple( -(i+1) for i in reversed(range(len(a.op.T.shape))) )
+    return _call_backend('nadd', [ast.Constant(value=dims), args[0]])
+
+@expr
+def nmax(a: Apply, args: List[ast.Name]) -> ast.expr:
+    assert type(a.op) == ops.NMax
+    assert len(args) == 1
+    # dimensions should be e.g., (-3, -2, -1) for
+    dims = tuple( -(i+1) for i in reversed(range(len(a.op.T.shape))) )
+    return _call_backend('nmax', [ast.Constant(value=dims), args[0]])
 
 @expr
 def negate(a: Apply, args: List[ast.Name]) -> ast.expr:
     assert type(a.op) == ops.Negate
     assert len(args) == 1
     return ast.UnaryOp(op=ast.USub(), operand=args[0])
 
 @expr
+def invert(a: Apply, args: List[ast.Name]) -> ast.expr:
+    assert type(a.op) == ops.Invert
+    assert len(args) == 1
+    return ast.UnaryOp(op=ast.Invert(), operand=args[0])
+
+@expr
 def divide(a: Apply, args: List[ast.Name]) -> ast.expr:
     assert type(a.op) == ops.Divide
     assert len(args) == 2
     b = ast.Div() if a.op.T.dtype.is_floating() else ast.FloorDiv()
     return ast.BinOp(left=args[0], op=b, right=args[1])
 
 @expr
 def constant(a: Apply, args: List[ast.Name]) -> ast.Call:
     assert type(a.op) == ops.Constant
     assert len(args) == 0
+    shape = ast.Tuple(
+            elts=[ ast.Constant(value=i) for i in a.op.T.shape ],
+            ctx=ast.Load())
     dtype = ast.Attribute(
             value=ast.Name(id="Dtype", ctx=ast.Load()),
             attr=a.op.T.dtype.name,
             ctx=ast.Load())
-    return _call_backend('constant', [ast.Constant(value=a.op.x), dtype])
+    return _call_backend('constant', [ast.Constant(value=a.op.x), shape, dtype])
 
 # An expression like self.backend.compose(x_0, x_1, 2)
 @expr
 def compose(a: Apply, args: List[ast.Name]) -> ast.Call:
     assert type(a.op) == ops.Compose
     assert len(args) == 2
     axes = len(a.op.B.shape)
@@ -133,94 +179,29 @@
     # permutation array as a constant expression
     p_arg = ast.List(elts=[ast.Constant(i, ctx=ast.Load()) for i in a.op.p], ctx=ast.Load())
     return _call_backend('permute', [ args[0], p_arg ])
 
 # Handlers for each operation
 # Each function here takes an Assignment ....
 OP_HANDLERS: dict[Type[operation], Callable[[Apply], List[ast.Assign]]] = {
+    # core operations
     ops.Copy: copy,
     ops.NCopy: ncopy,
+    ops.NSplit: nsplit,
+    ops.NConcatenate: nconcatenate,
     ops.Discard: discard,
     ops.Add: binop(ast.Add()),
     ops.NAdd: nadd,
+    ops.NMax: nmax,
     ops.Negate: negate,
+    ops.Invert: invert,
     ops.Subtract: binop(ast.Sub()),
     ops.Multiply: binop(ast.Mult()),
     ops.Divide: divide,
     ops.Power: binop(ast.Pow()),
     ops.Constant: constant,
+    ops.MatrixMultiply: binop(ast.MatMult()), # TODO: use binop matmult if len(B) == 1?
     ops.Compose: compose, # binop(ast.MatMult()), # TODO: use binop matmult if len(B) == 1?
     ops.Reshape: reshape,
     ops.Permute: permute,
+    ops.Gt: comparison(ast.Gt()),
 }
-
-################################################################################
-# Helpers to make python definitions
-
-def _mk_arguments(names: List[ast.Name]):
-    return ast.arguments(args=[ ast.arg(n) for n in names ], posonlyargs=[], kwonlyargs=[], kw_defaults=[], defaults=[])
-
-def _mk_module(name: str, fn_defs: List[ast.FunctionDef]) -> ast.Module:
-    _assert_identifier(name)
-    backend_assign = ast.AnnAssign(
-        target=ast.Name(id='backend', ctx=ast.Store()),
-        annotation=ast.Name(id='ArrayBackend', ctx=ast.Load()),
-        simple=1)
-
-    body = [backend_assign] + fn_defs
-
-    dc_import = ast.ImportFrom(module='dataclasses', names=[ast.alias(name='dataclass')], level=0)
-    cg_import = ast.ImportFrom(module='catgrad.signature', names=[ast.alias(name='Dtype')], level=0)
-    ab_import = ast.ImportFrom(module='catgrad.target.python.array_backend', names=[ast.alias(name='ArrayBackend')], level=0)
-    class_def = ast.ClassDef(
-            name=name,
-            bases=[],
-            keywords=[],
-            body=body,
-            decorator_list=[ast.Name(id="dataclass", ctx=ast.Load())],
-            type_params=[])
-
-    return ast.Module(body=[dc_import, cg_import, ab_import, class_def], type_ignores=[])
-
-def _mk_function_definition(f: OpenHypergraph, name: str = 'fn', op_handlers=OP_HANDLERS) -> ast.FunctionDef:
-    _assert_identifier(name)
-
-    # Get a catgrad FunctionDefinition
-    fn = FunctionDefinition.from_open_hypergraph(f)
-
-    # create a python FunctionDef
-    args = _mk_arguments(["self"] + [name_id(i) for i in fn.args])
-    body = [ assignment for apply in fn.body for assignment in op_handlers[type(apply.op)](apply) ]
-    rval = ast.List(elts=[ load(i) for i in fn.returns ], ctx=ast.Load())
-    body.append(ast.Return(value=rval, ctx=ast.Load()))
-    return ast.FunctionDef(
-        name = name,
-        args = args,
-        body = body,
-        decorator_list=[],
-        type_params=[])
-
-def to_python_class_ast(fs: dict[str, OpenHypergraph], class_name: str = 'Dynamic'):
-    fn_defs = {}
-    for name, f in fs.items():
-        _assert_identifier(name)
-        fn_defs[name] = _mk_function_definition(f, name)
-    mod_ast = _mk_module(class_name, list(fn_defs.values()))
-    ast.fix_missing_locations(mod_ast)
-    return mod_ast
-
-def to_python_class(fs: dict[str, OpenHypergraph], class_name: str = 'Dynamic'):
-    filename='<string>'
-    mod_ast = to_python_class_ast(fs, class_name)
-    env: Any = {}
-    exec(compile(mod_ast, filename=filename, mode='exec'), env)
-
-    # TODO: make tracebacks work properly for generated member functions.
-    return env[class_name]
-
-def to_python_function(f: OpenHypergraph, function_name: str = 'fn', filename='<string>', array_backend=Numpy) -> Callable:
-    # compile to a class
-    Dynamic = to_python_class({function_name: f}, 'Dynamic')
-
-    # instantiate with numpy array backend and return closure over class
-    d = Dynamic(Numpy)
-    return (lambda *args: d.fn(*args))
```

### Comparing `catgrad-0.1.0/LICENSE` & `catgrad-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catgrad-0.1.0/README.md` & `catgrad-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,58 @@
-# catgrad
+<div align="center">
+<img src="https://raw.githubusercontent.com/statusfailed/catgrad/master/docs/source/catgrad-logo.svg" height=200 />
+<h1>catgrad</h1>
+</div>
 
 You like category theory? You like tinygrad? You love catgrad! ❤️
 
 catgrad is a bit different: instead of using autograd to train, you *compile*
 your model's reverse pass into static code.
 This means your training loop can run without needing a deep learning framework
 (not even catgrad!)
 
-Here is a linear model in `catgrad`:
+Here is a linear model in catgrad:
 
-    model = layers.linear(BATCH_TYPE, INPUT_TYPE, OUTPUT_TYPE)
-
-catgrad can compile this model into static python code:
-
-    class CompiledModel:
-        backend: ArrayBackend
-
-        def predict(self, x1, x0):
-            x2 = x0 @ x1
-            return [x2]
-
-        def step(self, x0, x1, x9):
-            x4, x10 = (x0, x0)
-            x11, x12 = (x1, x1)
-            x16 = self.backend.constant(0.0001, Dtype.float32)
-            # ... snip ...
-            x18 = x17 * x5
-            x2 = x10 - x18
-            return [x2]
+```python
+model = layers.linear(BATCH_TYPE, INPUT_TYPE, OUTPUT_TYPE)
+```
+
+catgrad can compile this model...
+
+```python
+CompiledModel, _, _ = compile_model(model, layers.sgd(learning_rate), layers.mse)
+```
+
+... into static code like this...
+
+```python
+class CompiledModel:
+    backend: ArrayBackend
+
+    def predict(self, x1, x0):
+        x2 = x0 @ x1
+        return [x2]
+
+    def step(self, x0, x1, x9):
+        x4, x10 = (x0, x0)
+        x11, x12 = (x1, x1)
+        x16 = self.backend.constant(0.0001, Dtype.float32)
+        # ... snip ...
+        x18 = x17 * x5
+        x2 = x10 - x18
+        return [x2]
+```
 
 ... so you can train your model by just iterating `step`; no autograd needed:
 
     for i in range(0, NUM_ITER):
         p = step(p, x, y)
 
+Catgrad doesn't just compile to Python: I'm working on support for other targets like C++ (ggml), CUDA, FPGAs, and more!
+
 Catgrad uses [reverse derivatives](https://arxiv.org/abs/1910.07065)
 and [open hypergraphs](https://github.com/statusfailed/open-hypergraphs/)
 to transform a model into its backwards pass.
 For details, see [this paper](https://arxiv.org/abs/2305.01041).
 
 # Install
```

### Comparing `catgrad-0.1.0/pyproject.toml` & `catgrad-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "catgrad"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "deep learning with reverse derivatives"
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
```

### Comparing `catgrad-0.1.0/PKG-INFO` & `catgrad-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: catgrad
-Version: 0.1.0
+Version: 0.2.0
 Summary: deep learning with reverse derivatives
 Project-URL: Homepage, https://github.com/statusfailed/catgrad/
 Project-URL: Github, https://github.com/statusfailed/catgrad/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -13,50 +13,65 @@
 Requires-Dist: open-hypergraphs~=0.1.2
 Provides-Extra: dev
 Requires-Dist: hypothesis; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: scipy~=1.10.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# catgrad
+<div align="center">
+<img src="https://raw.githubusercontent.com/statusfailed/catgrad/master/docs/source/catgrad-logo.svg" height=200 />
+<h1>catgrad</h1>
+</div>
 
 You like category theory? You like tinygrad? You love catgrad! ❤️
 
 catgrad is a bit different: instead of using autograd to train, you *compile*
 your model's reverse pass into static code.
 This means your training loop can run without needing a deep learning framework
 (not even catgrad!)
 
-Here is a linear model in `catgrad`:
+Here is a linear model in catgrad:
 
-    model = layers.linear(BATCH_TYPE, INPUT_TYPE, OUTPUT_TYPE)
-
-catgrad can compile this model into static python code:
-
-    class CompiledModel:
-        backend: ArrayBackend
-
-        def predict(self, x1, x0):
-            x2 = x0 @ x1
-            return [x2]
-
-        def step(self, x0, x1, x9):
-            x4, x10 = (x0, x0)
-            x11, x12 = (x1, x1)
-            x16 = self.backend.constant(0.0001, Dtype.float32)
-            # ... snip ...
-            x18 = x17 * x5
-            x2 = x10 - x18
-            return [x2]
+```python
+model = layers.linear(BATCH_TYPE, INPUT_TYPE, OUTPUT_TYPE)
+```
+
+catgrad can compile this model...
+
+```python
+CompiledModel, _, _ = compile_model(model, layers.sgd(learning_rate), layers.mse)
+```
+
+... into static code like this...
+
+```python
+class CompiledModel:
+    backend: ArrayBackend
+
+    def predict(self, x1, x0):
+        x2 = x0 @ x1
+        return [x2]
+
+    def step(self, x0, x1, x9):
+        x4, x10 = (x0, x0)
+        x11, x12 = (x1, x1)
+        x16 = self.backend.constant(0.0001, Dtype.float32)
+        # ... snip ...
+        x18 = x17 * x5
+        x2 = x10 - x18
+        return [x2]
+```
 
 ... so you can train your model by just iterating `step`; no autograd needed:
 
     for i in range(0, NUM_ITER):
         p = step(p, x, y)
 
+Catgrad doesn't just compile to Python: I'm working on support for other targets like C++ (ggml), CUDA, FPGAs, and more!
+
 Catgrad uses [reverse derivatives](https://arxiv.org/abs/1910.07065)
 and [open hypergraphs](https://github.com/statusfailed/open-hypergraphs/)
 to transform a model into its backwards pass.
 For details, see [this paper](https://arxiv.org/abs/2305.01041).
 
 # Install
```

