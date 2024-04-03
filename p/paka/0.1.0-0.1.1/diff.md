# Comparing `tmp/paka-0.1.0.tar.gz` & `tmp/paka-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.0.tar", max compression
+gzip compressed data, was "paka-0.1.1.tar", max compression
```

## Comparing `paka-0.1.0.tar` & `paka-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1072 2024-02-20 22:26:59.896482 paka-0.1.0/LICENSE
--rw-r--r--   0        0        0     4071 2024-02-20 22:26:59.896482 paka-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-02-20 22:26:59.896482 paka-0.1.0/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/__init__.py
--rw-r--r--   0        0        0     1226 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/build.py
--rw-r--r--   0        0        0     2793 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/cluster.py
--rw-r--r--   0        0        0     6690 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/function.py
--rw-r--r--   0        0        0     5874 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2197 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/run.py
--rw-r--r--   0        0        0     8779 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    11885 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1432 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1874 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/keda.py
--rw-r--r--   0        0        0     4920 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2737 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/namespace.py
--rw-r--r--   0        0        0     4237 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-02-20 22:26:59.896482 paka-0.1.0/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    13265 2024-02-20 22:26:59.896482 paka-0.1.0/paka/config.py
--rw-r--r--   0        0        0      115 2024-02-20 22:26:59.896482 paka-0.1.0/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-02-20 22:26:59.896482 paka-0.1.0/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-02-20 22:26:59.896482 paka-0.1.0/paka/container/pack.py
--rw-r--r--   0        0        0    18963 2024-02-20 22:26:59.896482 paka-0.1.0/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5706 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     2012 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0     9969 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/model.py
--rw-r--r--   0        0        0    16598 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0     1105 2024-02-20 22:26:59.896482 paka-0.1.0/paka/kube_resources/model_group/supported_models.py
--rw-r--r--   0        0        0      761 2024-02-20 22:26:59.896482 paka-0.1.0/paka/logger.py
--rw-r--r--   0        0        0     9750 2024-02-20 22:26:59.896482 paka-0.1.0/paka/utils.py
--rw-r--r--   0        0        0     1262 2024-02-20 22:26:59.896482 paka-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 paka-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 04:57:05.293202 paka-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4445 2024-04-03 04:57:05.293202 paka-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-03 04:57:05.293202 paka-0.1.1/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/build.py
+-rw-r--r--   0        0        0     2793 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6690 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/function.py
+-rw-r--r--   0        0        0     5874 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/job.py
+-rw-r--r--   0        0        0      427 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2197 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3188 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/run.py
+-rw-r--r--   0        0        0     8779 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    11885 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1432 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1874 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4920 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2737 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     4237 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     4000 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    13265 2024-04-03 04:57:05.293202 paka-0.1.1/paka/config.py
+-rw-r--r--   0        0        0      115 2024-04-03 04:57:05.293202 paka-0.1.1/paka/constants.py
+-rw-r--r--   0        0        0     3015 2024-04-03 04:57:05.293202 paka-0.1.1/paka/container/ecr.py
+-rw-r--r--   0        0        0     2374 2024-04-03 04:57:05.293202 paka-0.1.1/paka/container/pack.py
+-rw-r--r--   0        0        0    18963 2024-04-03 04:57:05.293202 paka-0.1.1/paka/k8s.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/function/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/autoscaler.py
+-rw-r--r--   0        0        0     4142 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/__init__.py
+-rw-r--r--   0        0        0     2012 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/manifest.py
+-rw-r--r--   0        0        0     9969 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/model.py
+-rw-r--r--   0        0        0    16598 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/service.py
+-rw-r--r--   0        0        0     1105 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/supported_models.py
+-rw-r--r--   0        0        0      761 2024-04-03 04:57:05.293202 paka-0.1.1/paka/logger.py
+-rw-r--r--   0        0        0     9750 2024-04-03 04:57:05.293202 paka-0.1.1/paka/utils.py
+-rw-r--r--   0        0        0     1262 2024-04-03 04:57:05.293202 paka-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 paka-0.1.1/PKG-INFO
```

### Comparing `paka-0.1.0/LICENSE` & `paka-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/README.md` & `paka-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 ### Building
 Application, job code is built using [buildpacks](https://buildpacks.io/). No need to write Dockerfile. However, user still needs to have docker runtime installed.
 
 
 ## Paka CLI Reference
 
+Install the paka CLI
+```bash
+pip install paka
+```
+
 ### Provision a cluster
 
 Create a cluster.yaml
 ```yaml
 aws:
   cluster:
     name: example
@@ -84,11 +89,28 @@
 
 To deploy the application, run `paka function deploy --name <function_name> --source <source_path> --entrypoint <Procfile_command>. For example:
 
 ```bash
 paka function deploy --name langchain-server --source . --entrypoint serve
 ```
 
+### Destroy a cluster
+```bash
+paka cluster down -f cluster.yaml
+```
+
 ## Contributing
 - Open a PR
 - Format and lint code with `make lint`
 - Run tests with `make test`
+
+## Dependencies
+- docker daemon
+- aws cli and credentials for the AWS deployment
+```bash
+# Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
+# - S3
+# - ECR
+# - EKS
+# - EC2
+aws configure
+```
```

### Comparing `paka-0.1.0/paka/cli/__main__.py` & `paka-0.1.1/paka/cli/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 import typer
 
+from paka import __version__
 from paka.cli.build import build_app
 from paka.cli.cluster import cluster_app
 from paka.cli.function import function_app
 from paka.cli.job import job_app
 from paka.cli.kubeconfig import kube_app
 from paka.cli.model_group import model_group_app
 from paka.cli.run import run_app
 from paka.cli.utils import init_pulumi
 from paka.logger import setup_logger
 
 init_pulumi()
 
 
+def version_callback(version: bool) -> None:
+    if version:
+        typer.echo(f"Paka CLI Version: {__version__}")
+        raise typer.Exit()
+
+
 def verbose_option(
     verbose: bool = typer.Option(
         False, "--verbose", "-v", help="Enable verbose output"
     ),
 ) -> None:
     setup_logger(verbose)
 
 
 cli = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 cli.callback()(verbose_option)
 
+
+@cli.callback()
+def version_option(
+    ctx: typer.Context,
+    version: bool = typer.Option(
+        False, "--version", help="Show version and exit", callback=version_callback
+    ),
+) -> None:
+    pass
+
+
 cli.add_typer(cluster_app, name="cluster", help="Manage clusters.")
 
 cli.add_typer(job_app, name="job", help="Manage batch jobs.")
 
 cli.add_typer(build_app, name="build", help="Build Docker images.")
 
 cli.add_typer(kube_app, name="kubeconfig", help="Export kubeconfig.")
```

### Comparing `paka-0.1.0/paka/cli/build.py` & `paka-0.1.1/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/cluster.py` & `paka-0.1.1/paka/cli/cluster.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/function.py` & `paka-0.1.1/paka/cli/function.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/job.py` & `paka-0.1.1/paka/cli/job.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/model_group.py` & `paka-0.1.1/paka/cli/model_group.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/run.py` & `paka-0.1.1/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cli/utils.py` & `paka-0.1.1/paka/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/cloudwatch.py` & `paka-0.1.1/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.1/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/container_registry.py` & `paka-0.1.1/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.1/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/eks.py` & `paka-0.1.1/paka/cluster/aws/eks.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/elb.py` & `paka-0.1.1/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/object_store.py` & `paka-0.1.1/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/service_account.py` & `paka-0.1.1/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/aws/utils.py` & `paka-0.1.1/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/fluentbit.py` & `paka-0.1.1/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/keda.py` & `paka-0.1.1/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/knative.py` & `paka-0.1.1/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/manager/aws.py` & `paka-0.1.1/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/manager/base.py` & `paka-0.1.1/paka/cluster/manager/base.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/namespace.py` & `paka-0.1.1/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/prometheus.py` & `paka-0.1.1/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/qdrant.py` & `paka-0.1.1/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/redis.py` & `paka-0.1.1/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/cluster/zipkin.py` & `paka-0.1.1/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/config.py` & `paka-0.1.1/paka/config.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/container/ecr.py` & `paka-0.1.1/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/container/pack.py` & `paka-0.1.1/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/k8s.py` & `paka-0.1.1/paka/k8s.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/function/service.py` & `paka-0.1.1/paka/kube_resources/function/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/job/autoscaler.py` & `paka-0.1.1/paka/kube_resources/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/job/worker.py` & `paka-0.1.1/paka/kube_resources/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/model_group/ingress.py` & `paka-0.1.1/paka/kube_resources/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/model_group/model.py` & `paka-0.1.1/paka/kube_resources/model_group/model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/model_group/service.py` & `paka-0.1.1/paka/kube_resources/model_group/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/kube_resources/model_group/supported_models.py` & `paka-0.1.1/paka/kube_resources/model_group/supported_models.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/logger.py` & `paka-0.1.1/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/paka/utils.py` & `paka-0.1.1/paka/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.0/pyproject.toml` & `paka-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.0"
+version = "0.1.1"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
```

### Comparing `paka-0.1.0/PKG-INFO` & `paka-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.22,<2.0.0)
@@ -63,14 +63,19 @@
 
 ### Building
 Application, job code is built using [buildpacks](https://buildpacks.io/). No need to write Dockerfile. However, user still needs to have docker runtime installed.
 
 
 ## Paka CLI Reference
 
+Install the paka CLI
+```bash
+pip install paka
+```
+
 ### Provision a cluster
 
 Create a cluster.yaml
 ```yaml
 aws:
   cluster:
     name: example
@@ -108,12 +113,29 @@
 
 To deploy the application, run `paka function deploy --name <function_name> --source <source_path> --entrypoint <Procfile_command>. For example:
 
 ```bash
 paka function deploy --name langchain-server --source . --entrypoint serve
 ```
 
+### Destroy a cluster
+```bash
+paka cluster down -f cluster.yaml
+```
+
 ## Contributing
 - Open a PR
 - Format and lint code with `make lint`
 - Run tests with `make test`
 
+## Dependencies
+- docker daemon
+- aws cli and credentials for the AWS deployment
+```bash
+# Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
+# - S3
+# - ECR
+# - EKS
+# - EC2
+aws configure
+```
+
```

