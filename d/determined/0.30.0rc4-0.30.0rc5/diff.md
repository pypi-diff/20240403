# Comparing `tmp/determined-0.30.0rc4-py3-none-any.whl.zip` & `tmp/determined-0.30.0rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,273 +1,273 @@
-Zip file size: 681234 bytes, number of entries: 271
--rw-r--r--  2.0 unx     1140 b- defN 24-Mar-30 00:55 determined/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 24-Mar-30 00:55 determined/__version__.py
--rw-r--r--  2.0 unx     1664 b- defN 24-Mar-30 00:55 determined/_env_context.py
--rw-r--r--  2.0 unx     8854 b- defN 24-Mar-30 00:55 determined/_execution.py
--rw-r--r--  2.0 unx     2779 b- defN 24-Mar-30 00:55 determined/_experiment_config.py
--rw-r--r--  2.0 unx     4781 b- defN 24-Mar-30 00:55 determined/_import.py
--rw-r--r--  2.0 unx    14970 b- defN 24-Mar-30 00:55 determined/_info.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Mar-30 00:55 determined/_tf_rng.py
--rw-r--r--  2.0 unx     1220 b- defN 24-Mar-30 00:55 determined/_trial.py
--rw-r--r--  2.0 unx     4777 b- defN 24-Mar-30 00:55 determined/_trial_context.py
--rw-r--r--  2.0 unx     3246 b- defN 24-Mar-30 00:55 determined/_trial_controller.py
--rw-r--r--  2.0 unx     2271 b- defN 24-Mar-30 00:55 determined/constants.py
--rw-r--r--  2.0 unx     2734 b- defN 24-Mar-30 00:55 determined/errors.py
--rw-r--r--  2.0 unx     5627 b- defN 24-Mar-30 00:55 determined/gpu.py
--rw-r--r--  2.0 unx     6182 b- defN 24-Mar-30 00:55 determined/horovod.py
--rw-r--r--  2.0 unx    19947 b- defN 24-Mar-30 00:55 determined/ipc.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Mar-30 00:55 determined/load.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/py.typed
--rw-r--r--  2.0 unx    18236 b- defN 24-Mar-30 00:55 determined/util.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Mar-30 00:55 determined/workload.py
--rw-r--r--  2.0 unx      770 b- defN 24-Mar-30 00:55 determined/cli/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 24-Mar-30 00:55 determined/cli/__main__.py
--rw-r--r--  2.0 unx     4024 b- defN 24-Mar-30 00:55 determined/cli/_util.py
--rw-r--r--  2.0 unx     9943 b- defN 24-Mar-30 00:55 determined/cli/agent.py
--rw-r--r--  2.0 unx     8306 b- defN 24-Mar-30 00:55 determined/cli/checkpoint.py
--rw-r--r--  2.0 unx    12229 b- defN 24-Mar-30 00:55 determined/cli/cli.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Mar-30 00:55 determined/cli/command.py
--rw-r--r--  2.0 unx    11097 b- defN 24-Mar-30 00:55 determined/cli/dev.py
--rw-r--r--  2.0 unx      627 b- defN 24-Mar-30 00:55 determined/cli/errors.py
--rw-r--r--  2.0 unx    49692 b- defN 24-Mar-30 00:55 determined/cli/experiment.py
--rw-r--r--  2.0 unx     8772 b- defN 24-Mar-30 00:55 determined/cli/job.py
--rw-r--r--  2.0 unx     4409 b- defN 24-Mar-30 00:55 determined/cli/master.py
--rw-r--r--  2.0 unx     8446 b- defN 24-Mar-30 00:55 determined/cli/model.py
--rw-r--r--  2.0 unx     7017 b- defN 24-Mar-30 00:55 determined/cli/notebook.py
--rw-r--r--  2.0 unx    16642 b- defN 24-Mar-30 00:55 determined/cli/ntsc.py
--rw-r--r--  2.0 unx     1898 b- defN 24-Mar-30 00:55 determined/cli/oauth.py
--rw-r--r--  2.0 unx    11834 b- defN 24-Mar-30 00:55 determined/cli/project.py
--rw-r--r--  2.0 unx     7941 b- defN 24-Mar-30 00:55 determined/cli/proxy.py
--rw-r--r--  2.0 unx    18411 b- defN 24-Mar-30 00:55 determined/cli/rbac.py
--rw-r--r--  2.0 unx    10176 b- defN 24-Mar-30 00:55 determined/cli/render.py
--rw-r--r--  2.0 unx     4986 b- defN 24-Mar-30 00:55 determined/cli/resource_pool.py
--rw-r--r--  2.0 unx     2312 b- defN 24-Mar-30 00:55 determined/cli/resources.py
--rw-r--r--  2.0 unx    12944 b- defN 24-Mar-30 00:55 determined/cli/shell.py
--rw-r--r--  2.0 unx     5222 b- defN 24-Mar-30 00:55 determined/cli/sso.py
--rw-r--r--  2.0 unx    12820 b- defN 24-Mar-30 00:55 determined/cli/task.py
--rw-r--r--  2.0 unx     5206 b- defN 24-Mar-30 00:55 determined/cli/template.py
--rw-r--r--  2.0 unx     7560 b- defN 24-Mar-30 00:55 determined/cli/tensorboard.py
--rw-r--r--  2.0 unx      135 b- defN 24-Mar-30 00:55 determined/cli/top_arg_descriptions.py
--rw-r--r--  2.0 unx    16830 b- defN 24-Mar-30 00:55 determined/cli/trial.py
--rw-r--r--  2.0 unx     1635 b- defN 24-Mar-30 00:55 determined/cli/tunnel.py
--rw-r--r--  2.0 unx    10358 b- defN 24-Mar-30 00:55 determined/cli/user.py
--rw-r--r--  2.0 unx     8243 b- defN 24-Mar-30 00:55 determined/cli/user_groups.py
--rw-r--r--  2.0 unx     2577 b- defN 24-Mar-30 00:55 determined/cli/version.py
--rw-r--r--  2.0 unx    15298 b- defN 24-Mar-30 00:55 determined/cli/workspace.py
--rw-r--r--  2.0 unx      352 b- defN 24-Mar-30 00:55 determined/common/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 24-Mar-30 00:55 determined/common/_logging.py
--rw-r--r--  2.0 unx     8593 b- defN 24-Mar-30 00:55 determined/common/check.py
--rw-r--r--  2.0 unx     2154 b- defN 24-Mar-30 00:55 determined/common/constants.py
--rw-r--r--  2.0 unx     4278 b- defN 24-Mar-30 00:55 determined/common/context.py
--rw-r--r--  2.0 unx     8428 b- defN 24-Mar-30 00:55 determined/common/declarative_argparse.py
--rw-r--r--  2.0 unx     3569 b- defN 24-Mar-30 00:55 determined/common/detignore.py
--rw-r--r--  2.0 unx     3328 b- defN 24-Mar-30 00:55 determined/common/detlomond.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/common/py.typed
--rw-r--r--  2.0 unx     1662 b- defN 24-Mar-30 00:55 determined/common/requests.py
--rw-r--r--  2.0 unx    11922 b- defN 24-Mar-30 00:55 determined/common/util.py
--rw-r--r--  2.0 unx     1516 b- defN 24-Mar-30 00:55 determined/common/v1file_utils.py
--rw-r--r--  2.0 unx      809 b- defN 24-Mar-30 00:55 determined/common/api/__init__.py
--rw-r--r--  2.0 unx     4219 b- defN 24-Mar-30 00:55 determined/common/api/_rbac.py
--rw-r--r--  2.0 unx     8891 b- defN 24-Mar-30 00:55 determined/common/api/_session.py
--rw-r--r--  2.0 unx     6288 b- defN 24-Mar-30 00:55 determined/common/api/_util.py
--rw-r--r--  2.0 unx     1469 b- defN 24-Mar-30 00:55 determined/common/api/analytics.py
--rw-r--r--  2.0 unx    21290 b- defN 24-Mar-30 00:55 determined/common/api/authentication.py
--rw-r--r--  2.0 unx   809512 b- defN 24-Mar-30 00:55 determined/common/api/bindings.py
--rw-r--r--  2.0 unx     7421 b- defN 24-Mar-30 00:55 determined/common/api/certs.py
--rw-r--r--  2.0 unx     3773 b- defN 24-Mar-30 00:55 determined/common/api/errors.py
--rw-r--r--  2.0 unx     3281 b- defN 24-Mar-30 00:55 determined/common/api/logs.py
--rw-r--r--  2.0 unx      247 b- defN 24-Mar-30 00:55 determined/common/api/metric.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Mar-30 00:55 determined/common/experimental/__init__.py
--rw-r--r--  2.0 unx      465 b- defN 24-Mar-30 00:55 determined/common/experimental/_util.py
--rw-r--r--  2.0 unx    22742 b- defN 24-Mar-30 00:55 determined/common/experimental/determined.py
--rw-r--r--  2.0 unx    26924 b- defN 24-Mar-30 00:55 determined/common/experimental/experiment.py
--rw-r--r--  2.0 unx     3567 b- defN 24-Mar-30 00:55 determined/common/experimental/metrics.py
--rw-r--r--  2.0 unx    16083 b- defN 24-Mar-30 00:55 determined/common/experimental/model.py
--rw-r--r--  2.0 unx      306 b- defN 24-Mar-30 00:55 determined/common/experimental/oauth2_scim_client.py
--rw-r--r--  2.0 unx     7712 b- defN 24-Mar-30 00:55 determined/common/experimental/project.py
--rw-r--r--  2.0 unx     3607 b- defN 24-Mar-30 00:55 determined/common/experimental/resource_pool.py
--rw-r--r--  2.0 unx    25595 b- defN 24-Mar-30 00:55 determined/common/experimental/trial.py
--rw-r--r--  2.0 unx     4750 b- defN 24-Mar-30 00:55 determined/common/experimental/user.py
--rw-r--r--  2.0 unx     5801 b- defN 24-Mar-30 00:55 determined/common/experimental/workspace.py
--rw-r--r--  2.0 unx      170 b- defN 24-Mar-30 00:55 determined/common/experimental/checkpoint/__init__.py
--rw-r--r--  2.0 unx    20350 b- defN 24-Mar-30 00:55 determined/common/experimental/checkpoint/_checkpoint.py
--rw-r--r--  2.0 unx     4094 b- defN 24-Mar-30 00:55 determined/common/storage/__init__.py
--rw-r--r--  2.0 unx     4339 b- defN 24-Mar-30 00:55 determined/common/storage/azure.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Mar-30 00:55 determined/common/storage/azure_client.py
--rw-r--r--  2.0 unx     9368 b- defN 24-Mar-30 00:55 determined/common/storage/base.py
--rw-r--r--  2.0 unx     4506 b- defN 24-Mar-30 00:55 determined/common/storage/boto3_credential_manager.py
--rw-r--r--  2.0 unx     1014 b- defN 24-Mar-30 00:55 determined/common/storage/cloud.py
--rw-r--r--  2.0 unx     2282 b- defN 24-Mar-30 00:55 determined/common/storage/directory.py
--rw-r--r--  2.0 unx     6529 b- defN 24-Mar-30 00:55 determined/common/storage/gcs.py
--rw-r--r--  2.0 unx     6702 b- defN 24-Mar-30 00:55 determined/common/storage/s3.py
--rw-r--r--  2.0 unx     9868 b- defN 24-Mar-30 00:55 determined/common/storage/shared.py
--rw-r--r--  2.0 unx      243 b- defN 24-Mar-30 00:55 determined/common/streams/__init__.py
--rw-r--r--  2.0 unx    18251 b- defN 24-Mar-30 00:55 determined/common/streams/_client.py
--rw-r--r--  2.0 unx      391 b- defN 24-Mar-30 00:55 determined/common/streams/_util.py
--rw-r--r--  2.0 unx     3899 b- defN 24-Mar-30 00:55 determined/common/streams/wire.py
--rw-r--r--  2.0 unx     1315 b- defN 24-Mar-30 00:55 determined/core/__init__.py
--rw-r--r--  2.0 unx    30354 b- defN 24-Mar-30 00:55 determined/core/_checkpoint.py
--rw-r--r--  2.0 unx    14071 b- defN 24-Mar-30 00:55 determined/core/_context.py
--rw-r--r--  2.0 unx    16604 b- defN 24-Mar-30 00:55 determined/core/_distributed.py
--rw-r--r--  2.0 unx     2884 b- defN 24-Mar-30 00:55 determined/core/_experimental.py
--rw-r--r--  2.0 unx     4831 b- defN 24-Mar-30 00:55 determined/core/_heartbeat.py
--rw-r--r--  2.0 unx     5680 b- defN 24-Mar-30 00:55 determined/core/_log_shipper.py
--rw-r--r--  2.0 unx    12734 b- defN 24-Mar-30 00:55 determined/core/_preempt.py
--rw-r--r--  2.0 unx    17194 b- defN 24-Mar-30 00:55 determined/core/_profiler.py
--rw-r--r--  2.0 unx    15041 b- defN 24-Mar-30 00:55 determined/core/_searcher.py
--rw-r--r--  2.0 unx      932 b- defN 24-Mar-30 00:55 determined/core/_tensorboard_mode.py
--rw-r--r--  2.0 unx    12099 b- defN 24-Mar-30 00:55 determined/core/_train.py
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-30 00:55 determined/deploy/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Mar-30 00:55 determined/deploy/cli.py
--rw-r--r--  2.0 unx      855 b- defN 24-Mar-30 00:55 determined/deploy/errors.py
--rw-r--r--  2.0 unx     2109 b- defN 24-Mar-30 00:55 determined/deploy/healthcheck.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/aws/__init__.py
--rw-r--r--  2.0 unx    19768 b- defN 24-Mar-30 00:55 determined/deploy/aws/aws.py
--rw-r--r--  2.0 unx    29160 b- defN 24-Mar-30 00:55 determined/deploy/aws/cli.py
--rw-r--r--  2.0 unx     3322 b- defN 24-Mar-30 00:55 determined/deploy/aws/constants.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Mar-30 00:55 determined/deploy/aws/gen_vcpu_mapping.py
--rw-r--r--  2.0 unx     2201 b- defN 24-Mar-30 00:55 determined/deploy/aws/master_config_inject.py
--rw-r--r--  2.0 unx     5193 b- defN 24-Mar-30 00:55 determined/deploy/aws/preflight.py
--rw-r--r--  2.0 unx    17324 b- defN 24-Mar-30 00:55 determined/deploy/aws/vcpu_mapping.yaml
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/__init__.py
--rw-r--r--  2.0 unx     5961 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/base.py
--rw-r--r--  2.0 unx     1593 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/govcloud.py
--rw-r--r--  2.0 unx     3094 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/secure.py
--rw-r--r--  2.0 unx     1886 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/simple.py
--rw-r--r--  2.0 unx     2381 b- defN 24-Mar-30 00:55 determined/deploy/aws/deployment_types/vpc.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/__init__.py
--rw-r--r--  2.0 unx    30153 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/efs.yaml
--rw-r--r--  2.0 unx    30863 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/fsx.yaml
--rw-r--r--  2.0 unx    24489 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/govcloud.yaml
--rw-r--r--  2.0 unx    32137 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/lore.yaml
--rw-r--r--  2.0 unx    30025 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/secure.yaml
--rw-r--r--  2.0 unx    26082 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/simple-rds.yaml
--rw-r--r--  2.0 unx    25798 b- defN 24-Mar-30 00:55 determined/deploy/aws/templates/simple.yaml
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/gcp/__init__.py
--rw-r--r--  2.0 unx    25487 b- defN 24-Mar-30 00:55 determined/deploy/gcp/cli.py
--rw-r--r--  2.0 unx      771 b- defN 24-Mar-30 00:55 determined/deploy/gcp/constants.py
--rw-r--r--  2.0 unx    15099 b- defN 24-Mar-30 00:55 determined/deploy/gcp/gcp.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Mar-30 00:55 determined/deploy/gcp/preflight.py
--rw-r--r--  2.0 unx     5428 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/main.tf
--rw-r--r--  2.0 unx     1647 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/master.yaml.tmpl
--rw-r--r--  2.0 unx     1487 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/outputs.tf
--rw-r--r--  2.0 unx     3836 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/variables.tf
--rw-r--r--  2.0 unx     6195 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/compute/main.tf
--rw-r--r--  2.0 unx      424 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/compute/outputs.tf
--rw-r--r--  2.0 unx     1612 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/compute/variables.tf
--rw-r--r--  2.0 unx     1222 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/database/main.tf
--rw-r--r--  2.0 unx      283 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/database/outputs.tf
--rw-r--r--  2.0 unx      320 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/database/variables.tf
--rw-r--r--  2.0 unx      522 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/filestore/main.tf
--rw-r--r--  2.0 unx      184 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
--rw-r--r--  2.0 unx      125 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/filestore/variables.tf
--rw-r--r--  2.0 unx     1026 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/firewall/main.tf
--rw-r--r--  2.0 unx      195 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
--rw-r--r--  2.0 unx       75 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/firewall/variables.tf
--rw-r--r--  2.0 unx      637 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/gcs/main.tf
--rw-r--r--  2.0 unx       51 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
--rw-r--r--  2.0 unx      161 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/gcs/variables.tf
--rw-r--r--  2.0 unx      161 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/ip/main.tf
--rw-r--r--  2.0 unx      122 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/ip/outputs.tf
--rw-r--r--  2.0 unx       88 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/ip/variables.tf
--rw-r--r--  2.0 unx     1112 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/network/main.tf
--rw-r--r--  2.0 unx      275 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/network/outputs.tf
--rw-r--r--  2.0 unx      207 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/network/variables.tf
--rw-r--r--  2.0 unx      962 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/service_account/main.tf
--rw-r--r--  2.0 unx       73 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
--rw-r--r--  2.0 unx      138 b- defN 24-Mar-30 00:55 determined/deploy/gcp/terraform/modules/service_account/variables.tf
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/gke/__init__.py
--rw-r--r--  2.0 unx    19671 b- defN 24-Mar-30 00:55 determined/deploy/gke/cli.py
--rw-r--r--  2.0 unx      408 b- defN 24-Mar-30 00:55 determined/deploy/gke/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/deploy/local/__init__.py
--rw-r--r--  2.0 unx    13137 b- defN 24-Mar-30 00:55 determined/deploy/local/cli.py
--rw-r--r--  2.0 unx    17119 b- defN 24-Mar-30 00:55 determined/deploy/local/cluster_utils.py
--rw-r--r--  2.0 unx     1134 b- defN 24-Mar-30 00:55 determined/deploy/local/preflight.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/exec/__init__.py
--rw-r--r--  2.0 unx     5473 b- defN 24-Mar-30 00:55 determined/exec/gc_checkpoints.py
--rw-r--r--  2.0 unx     8475 b- defN 24-Mar-30 00:55 determined/exec/harness.py
--rw-r--r--  2.0 unx     3695 b- defN 24-Mar-30 00:55 determined/exec/launch.py
--rw-r--r--  2.0 unx      389 b- defN 24-Mar-30 00:55 determined/exec/pid_client.py
--rw-r--r--  2.0 unx     1718 b- defN 24-Mar-30 00:55 determined/exec/pid_server.py
--rw-r--r--  2.0 unx    13760 b- defN 24-Mar-30 00:55 determined/exec/prep_container.py
--rw-r--r--  2.0 unx    11234 b- defN 24-Mar-30 00:55 determined/exec/tensorboard.py
--rw-r--r--  2.0 unx      611 b- defN 24-Mar-30 00:55 determined/experimental/__init__.py
--rw-r--r--  2.0 unx     3536 b- defN 24-Mar-30 00:55 determined/experimental/_native.py
--rw-r--r--  2.0 unx    22391 b- defN 24-Mar-30 00:55 determined/experimental/client.py
--rw-r--r--  2.0 unx      959 b- defN 24-Mar-30 00:55 determined/experimental/core_v2/__init__.py
--rw-r--r--  2.0 unx     6260 b- defN 24-Mar-30 00:55 determined/experimental/core_v2/_core_context_v2.py
--rw-r--r--  2.0 unx     8851 b- defN 24-Mar-30 00:55 determined/experimental/core_v2/_core_v2.py
--rw-r--r--  2.0 unx     9851 b- defN 24-Mar-30 00:55 determined/experimental/core_v2/_unmanaged.py
--rw-r--r--  2.0 unx      744 b- defN 24-Mar-30 00:55 determined/keras/__init__.py
--rw-r--r--  2.0 unx     7579 b- defN 24-Mar-30 00:55 determined/keras/_data.py
--rw-r--r--  2.0 unx    11491 b- defN 24-Mar-30 00:55 determined/keras/_enqueuer.py
--rw-r--r--  2.0 unx     4066 b- defN 24-Mar-30 00:55 determined/keras/_load.py
--rw-r--r--  2.0 unx      533 b- defN 24-Mar-30 00:55 determined/keras/_tensorboard_callback.py
--rw-r--r--  2.0 unx    19081 b- defN 24-Mar-30 00:55 determined/keras/_tf_keras_context.py
--rw-r--r--  2.0 unx     1251 b- defN 24-Mar-30 00:55 determined/keras/_tf_keras_multi_gpu.py
--rw-r--r--  2.0 unx    47995 b- defN 24-Mar-30 00:55 determined/keras/_tf_keras_trial.py
--rw-r--r--  2.0 unx    27517 b- defN 24-Mar-30 00:55 determined/keras/callbacks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/launch/__init__.py
--rw-r--r--  2.0 unx    15109 b- defN 24-Mar-30 00:55 determined/launch/deepspeed.py
--rw-r--r--  2.0 unx    10780 b- defN 24-Mar-30 00:55 determined/launch/horovod.py
--rw-r--r--  2.0 unx     4640 b- defN 24-Mar-30 00:55 determined/launch/torch_distributed.py
--rw-r--r--  2.0 unx     6831 b- defN 24-Mar-30 00:55 determined/launch/wrap_rank.py
--rw-r--r--  2.0 unx       98 b- defN 24-Mar-30 00:55 determined/layers/__init__.py
--rw-r--r--  2.0 unx    19697 b- defN 24-Mar-30 00:55 determined/layers/_workload_sequencer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:55 determined/lightning/__init__.py
--rw-r--r--  2.0 unx     1847 b- defN 24-Mar-30 00:55 determined/lightning/experimental.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Mar-30 00:55 determined/pytorch/__init__.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Mar-30 00:55 determined/pytorch/_callback.py
--rw-r--r--  2.0 unx    16717 b- defN 24-Mar-30 00:55 determined/pytorch/_data.py
--rw-r--r--  2.0 unx     3716 b- defN 24-Mar-30 00:55 determined/pytorch/_experimental.py
--rw-r--r--  2.0 unx    12557 b- defN 24-Mar-30 00:55 determined/pytorch/_load.py
--rw-r--r--  2.0 unx     3286 b- defN 24-Mar-30 00:55 determined/pytorch/_lr_scheduler.py
--rw-r--r--  2.0 unx     8322 b- defN 24-Mar-30 00:55 determined/pytorch/_metric_utils.py
--rw-r--r--  2.0 unx    46422 b- defN 24-Mar-30 00:55 determined/pytorch/_pytorch_context.py
--rw-r--r--  2.0 unx    68495 b- defN 24-Mar-30 00:55 determined/pytorch/_pytorch_trial.py
--rw-r--r--  2.0 unx    21628 b- defN 24-Mar-30 00:55 determined/pytorch/_reducer.py
--rw-r--r--  2.0 unx    14449 b- defN 24-Mar-30 00:55 determined/pytorch/_trainer.py
--rw-r--r--  2.0 unx     9561 b- defN 24-Mar-30 00:55 determined/pytorch/samplers.py
--rw-r--r--  2.0 unx      347 b- defN 24-Mar-30 00:55 determined/pytorch/deepspeed/__init__.py
--rw-r--r--  2.0 unx    19896 b- defN 24-Mar-30 00:55 determined/pytorch/deepspeed/_deepspeed_context.py
--rw-r--r--  2.0 unx    43012 b- defN 24-Mar-30 00:55 determined/pytorch/deepspeed/_deepspeed_trial.py
--rw-r--r--  2.0 unx     1987 b- defN 24-Mar-30 00:55 determined/pytorch/deepspeed/_mpu.py
--rw-r--r--  2.0 unx      409 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/__main__.py
--rw-r--r--  2.0 unx     2541 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/_defaults.py
--rw-r--r--  2.0 unx    60179 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/_dsat_search_method.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/_run_dsat.py
--rw-r--r--  2.0 unx    20150 b- defN 24-Mar-30 00:55 determined/pytorch/dsat/_utils.py
--rw-r--r--  2.0 unx      175 b- defN 24-Mar-30 00:55 determined/pytorch/experimental/__init__.py
--rw-r--r--  2.0 unx    21611 b- defN 24-Mar-30 00:55 determined/pytorch/experimental/_torch_batch_process.py
--rw-r--r--  2.0 unx      343 b- defN 24-Mar-30 00:55 determined/searcher/__init__.py
--rw-r--r--  2.0 unx     4134 b- defN 24-Mar-30 00:55 determined/searcher/_remote_search_runner.py
--rw-r--r--  2.0 unx    16436 b- defN 24-Mar-30 00:55 determined/searcher/_search_method.py
--rw-r--r--  2.0 unx    15961 b- defN 24-Mar-30 00:55 determined/searcher/_search_runner.py
--rw-r--r--  2.0 unx      512 b- defN 24-Mar-30 00:55 determined/tensorboard/__init__.py
--rw-r--r--  2.0 unx     1579 b- defN 24-Mar-30 00:55 determined/tensorboard/azure.py
--rw-r--r--  2.0 unx     6111 b- defN 24-Mar-30 00:55 determined/tensorboard/base.py
--rw-r--r--  2.0 unx     4641 b- defN 24-Mar-30 00:55 determined/tensorboard/build.py
--rw-r--r--  2.0 unx      225 b- defN 24-Mar-30 00:55 determined/tensorboard/directory.py
--rw-r--r--  2.0 unx     2357 b- defN 24-Mar-30 00:55 determined/tensorboard/gcs.py
--rw-r--r--  2.0 unx     1895 b- defN 24-Mar-30 00:55 determined/tensorboard/s3.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Mar-30 00:55 determined/tensorboard/shared.py
--rw-r--r--  2.0 unx     3787 b- defN 24-Mar-30 00:55 determined/tensorboard/util.py
--rw-r--r--  2.0 unx      845 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/__init__.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/azure.py
--rw-r--r--  2.0 unx     1670 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/base.py
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/directory.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/gcs.py
--rw-r--r--  2.0 unx     2495 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/s3.py
--rw-r--r--  2.0 unx     1657 b- defN 24-Mar-30 00:55 determined/tensorboard/fetchers/shared.py
--rw-r--r--  2.0 unx       91 b- defN 24-Mar-30 00:55 determined/tensorboard/metric_writers/__init__.py
--rw-r--r--  2.0 unx     3313 b- defN 24-Mar-30 00:55 determined/tensorboard/metric_writers/callback.py
--rw-r--r--  2.0 unx     3255 b- defN 24-Mar-30 00:55 determined/tensorboard/metric_writers/pytorch.py
--rw-r--r--  2.0 unx     4443 b- defN 24-Mar-30 00:55 determined/tensorboard/metric_writers/tensorflow.py
--rw-r--r--  2.0 unx       70 b- defN 24-Mar-30 00:55 determined/transformers/__init__.py
--rw-r--r--  2.0 unx    12730 b- defN 24-Mar-30 00:55 determined/transformers/_hf_callback.py
--rw-r--r--  2.0 unx     1242 b- defN 24-Mar-30 00:55 determined-0.30.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-30 00:55 determined-0.30.0rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Mar-30 00:55 determined-0.30.0rc4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-30 00:55 determined-0.30.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    24976 b- defN 24-Mar-30 00:55 determined-0.30.0rc4.dist-info/RECORD
-271 files, 2880438 bytes uncompressed, 641386 bytes compressed:  77.7%
+Zip file size: 681232 bytes, number of entries: 271
+-rw-r--r--  2.0 unx     1140 b- defN 24-Apr-03 21:38 determined/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-03 21:38 determined/__version__.py
+-rw-r--r--  2.0 unx     1664 b- defN 24-Apr-03 21:38 determined/_env_context.py
+-rw-r--r--  2.0 unx     8854 b- defN 24-Apr-03 21:38 determined/_execution.py
+-rw-r--r--  2.0 unx     2779 b- defN 24-Apr-03 21:38 determined/_experiment_config.py
+-rw-r--r--  2.0 unx     4781 b- defN 24-Apr-03 21:38 determined/_import.py
+-rw-r--r--  2.0 unx    14970 b- defN 24-Apr-03 21:38 determined/_info.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-03 21:38 determined/_tf_rng.py
+-rw-r--r--  2.0 unx     1220 b- defN 24-Apr-03 21:38 determined/_trial.py
+-rw-r--r--  2.0 unx     4777 b- defN 24-Apr-03 21:38 determined/_trial_context.py
+-rw-r--r--  2.0 unx     3246 b- defN 24-Apr-03 21:38 determined/_trial_controller.py
+-rw-r--r--  2.0 unx     2271 b- defN 24-Apr-03 21:38 determined/constants.py
+-rw-r--r--  2.0 unx     2734 b- defN 24-Apr-03 21:38 determined/errors.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-Apr-03 21:38 determined/gpu.py
+-rw-r--r--  2.0 unx     6182 b- defN 24-Apr-03 21:38 determined/horovod.py
+-rw-r--r--  2.0 unx    19947 b- defN 24-Apr-03 21:38 determined/ipc.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-03 21:38 determined/load.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/py.typed
+-rw-r--r--  2.0 unx    18236 b- defN 24-Apr-03 21:38 determined/util.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Apr-03 21:38 determined/workload.py
+-rw-r--r--  2.0 unx      770 b- defN 24-Apr-03 21:38 determined/cli/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 24-Apr-03 21:38 determined/cli/__main__.py
+-rw-r--r--  2.0 unx     4024 b- defN 24-Apr-03 21:38 determined/cli/_util.py
+-rw-r--r--  2.0 unx     9943 b- defN 24-Apr-03 21:38 determined/cli/agent.py
+-rw-r--r--  2.0 unx     8306 b- defN 24-Apr-03 21:38 determined/cli/checkpoint.py
+-rw-r--r--  2.0 unx    12229 b- defN 24-Apr-03 21:38 determined/cli/cli.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-03 21:38 determined/cli/command.py
+-rw-r--r--  2.0 unx    11097 b- defN 24-Apr-03 21:38 determined/cli/dev.py
+-rw-r--r--  2.0 unx      627 b- defN 24-Apr-03 21:38 determined/cli/errors.py
+-rw-r--r--  2.0 unx    49692 b- defN 24-Apr-03 21:38 determined/cli/experiment.py
+-rw-r--r--  2.0 unx     8772 b- defN 24-Apr-03 21:38 determined/cli/job.py
+-rw-r--r--  2.0 unx     4409 b- defN 24-Apr-03 21:38 determined/cli/master.py
+-rw-r--r--  2.0 unx     8446 b- defN 24-Apr-03 21:38 determined/cli/model.py
+-rw-r--r--  2.0 unx     7017 b- defN 24-Apr-03 21:38 determined/cli/notebook.py
+-rw-r--r--  2.0 unx    16642 b- defN 24-Apr-03 21:38 determined/cli/ntsc.py
+-rw-r--r--  2.0 unx     1898 b- defN 24-Apr-03 21:38 determined/cli/oauth.py
+-rw-r--r--  2.0 unx    11834 b- defN 24-Apr-03 21:38 determined/cli/project.py
+-rw-r--r--  2.0 unx     7941 b- defN 24-Apr-03 21:38 determined/cli/proxy.py
+-rw-r--r--  2.0 unx    18411 b- defN 24-Apr-03 21:38 determined/cli/rbac.py
+-rw-r--r--  2.0 unx    10176 b- defN 24-Apr-03 21:38 determined/cli/render.py
+-rw-r--r--  2.0 unx     4986 b- defN 24-Apr-03 21:38 determined/cli/resource_pool.py
+-rw-r--r--  2.0 unx     2312 b- defN 24-Apr-03 21:38 determined/cli/resources.py
+-rw-r--r--  2.0 unx    12944 b- defN 24-Apr-03 21:38 determined/cli/shell.py
+-rw-r--r--  2.0 unx     5222 b- defN 24-Apr-03 21:38 determined/cli/sso.py
+-rw-r--r--  2.0 unx    12820 b- defN 24-Apr-03 21:38 determined/cli/task.py
+-rw-r--r--  2.0 unx     5206 b- defN 24-Apr-03 21:38 determined/cli/template.py
+-rw-r--r--  2.0 unx     7560 b- defN 24-Apr-03 21:38 determined/cli/tensorboard.py
+-rw-r--r--  2.0 unx      135 b- defN 24-Apr-03 21:38 determined/cli/top_arg_descriptions.py
+-rw-r--r--  2.0 unx    16830 b- defN 24-Apr-03 21:38 determined/cli/trial.py
+-rw-r--r--  2.0 unx     1635 b- defN 24-Apr-03 21:38 determined/cli/tunnel.py
+-rw-r--r--  2.0 unx    10358 b- defN 24-Apr-03 21:38 determined/cli/user.py
+-rw-r--r--  2.0 unx     8243 b- defN 24-Apr-03 21:38 determined/cli/user_groups.py
+-rw-r--r--  2.0 unx     2577 b- defN 24-Apr-03 21:38 determined/cli/version.py
+-rw-r--r--  2.0 unx    15298 b- defN 24-Apr-03 21:38 determined/cli/workspace.py
+-rw-r--r--  2.0 unx      352 b- defN 24-Apr-03 21:38 determined/common/__init__.py
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-03 21:38 determined/common/_logging.py
+-rw-r--r--  2.0 unx     8593 b- defN 24-Apr-03 21:38 determined/common/check.py
+-rw-r--r--  2.0 unx     2154 b- defN 24-Apr-03 21:38 determined/common/constants.py
+-rw-r--r--  2.0 unx     4278 b- defN 24-Apr-03 21:38 determined/common/context.py
+-rw-r--r--  2.0 unx     8428 b- defN 24-Apr-03 21:38 determined/common/declarative_argparse.py
+-rw-r--r--  2.0 unx     3569 b- defN 24-Apr-03 21:38 determined/common/detignore.py
+-rw-r--r--  2.0 unx     3328 b- defN 24-Apr-03 21:38 determined/common/detlomond.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/common/py.typed
+-rw-r--r--  2.0 unx     1662 b- defN 24-Apr-03 21:38 determined/common/requests.py
+-rw-r--r--  2.0 unx    11922 b- defN 24-Apr-03 21:38 determined/common/util.py
+-rw-r--r--  2.0 unx     1516 b- defN 24-Apr-03 21:38 determined/common/v1file_utils.py
+-rw-r--r--  2.0 unx      809 b- defN 24-Apr-03 21:38 determined/common/api/__init__.py
+-rw-r--r--  2.0 unx     4219 b- defN 24-Apr-03 21:38 determined/common/api/_rbac.py
+-rw-r--r--  2.0 unx     8891 b- defN 24-Apr-03 21:38 determined/common/api/_session.py
+-rw-r--r--  2.0 unx     6288 b- defN 24-Apr-03 21:38 determined/common/api/_util.py
+-rw-r--r--  2.0 unx     1469 b- defN 24-Apr-03 21:38 determined/common/api/analytics.py
+-rw-r--r--  2.0 unx    21290 b- defN 24-Apr-03 21:38 determined/common/api/authentication.py
+-rw-r--r--  2.0 unx   809512 b- defN 24-Apr-03 21:38 determined/common/api/bindings.py
+-rw-r--r--  2.0 unx     7421 b- defN 24-Apr-03 21:38 determined/common/api/certs.py
+-rw-r--r--  2.0 unx     3773 b- defN 24-Apr-03 21:38 determined/common/api/errors.py
+-rw-r--r--  2.0 unx     3281 b- defN 24-Apr-03 21:38 determined/common/api/logs.py
+-rw-r--r--  2.0 unx      247 b- defN 24-Apr-03 21:38 determined/common/api/metric.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-03 21:38 determined/common/experimental/__init__.py
+-rw-r--r--  2.0 unx      465 b- defN 24-Apr-03 21:38 determined/common/experimental/_util.py
+-rw-r--r--  2.0 unx    22742 b- defN 24-Apr-03 21:38 determined/common/experimental/determined.py
+-rw-r--r--  2.0 unx    26924 b- defN 24-Apr-03 21:38 determined/common/experimental/experiment.py
+-rw-r--r--  2.0 unx     3567 b- defN 24-Apr-03 21:38 determined/common/experimental/metrics.py
+-rw-r--r--  2.0 unx    16083 b- defN 24-Apr-03 21:38 determined/common/experimental/model.py
+-rw-r--r--  2.0 unx      306 b- defN 24-Apr-03 21:38 determined/common/experimental/oauth2_scim_client.py
+-rw-r--r--  2.0 unx     7712 b- defN 24-Apr-03 21:38 determined/common/experimental/project.py
+-rw-r--r--  2.0 unx     3607 b- defN 24-Apr-03 21:38 determined/common/experimental/resource_pool.py
+-rw-r--r--  2.0 unx    25595 b- defN 24-Apr-03 21:38 determined/common/experimental/trial.py
+-rw-r--r--  2.0 unx     4750 b- defN 24-Apr-03 21:38 determined/common/experimental/user.py
+-rw-r--r--  2.0 unx     5801 b- defN 24-Apr-03 21:38 determined/common/experimental/workspace.py
+-rw-r--r--  2.0 unx      170 b- defN 24-Apr-03 21:38 determined/common/experimental/checkpoint/__init__.py
+-rw-r--r--  2.0 unx    20350 b- defN 24-Apr-03 21:38 determined/common/experimental/checkpoint/_checkpoint.py
+-rw-r--r--  2.0 unx     4094 b- defN 24-Apr-03 21:38 determined/common/storage/__init__.py
+-rw-r--r--  2.0 unx     4339 b- defN 24-Apr-03 21:38 determined/common/storage/azure.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-Apr-03 21:38 determined/common/storage/azure_client.py
+-rw-r--r--  2.0 unx     9368 b- defN 24-Apr-03 21:38 determined/common/storage/base.py
+-rw-r--r--  2.0 unx     4506 b- defN 24-Apr-03 21:38 determined/common/storage/boto3_credential_manager.py
+-rw-r--r--  2.0 unx     1014 b- defN 24-Apr-03 21:38 determined/common/storage/cloud.py
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-03 21:38 determined/common/storage/directory.py
+-rw-r--r--  2.0 unx     6529 b- defN 24-Apr-03 21:38 determined/common/storage/gcs.py
+-rw-r--r--  2.0 unx     6702 b- defN 24-Apr-03 21:38 determined/common/storage/s3.py
+-rw-r--r--  2.0 unx     9868 b- defN 24-Apr-03 21:38 determined/common/storage/shared.py
+-rw-r--r--  2.0 unx      243 b- defN 24-Apr-03 21:38 determined/common/streams/__init__.py
+-rw-r--r--  2.0 unx    18251 b- defN 24-Apr-03 21:38 determined/common/streams/_client.py
+-rw-r--r--  2.0 unx      391 b- defN 24-Apr-03 21:38 determined/common/streams/_util.py
+-rw-r--r--  2.0 unx     3899 b- defN 24-Apr-03 21:38 determined/common/streams/wire.py
+-rw-r--r--  2.0 unx     1315 b- defN 24-Apr-03 21:38 determined/core/__init__.py
+-rw-r--r--  2.0 unx    30354 b- defN 24-Apr-03 21:38 determined/core/_checkpoint.py
+-rw-r--r--  2.0 unx    14071 b- defN 24-Apr-03 21:38 determined/core/_context.py
+-rw-r--r--  2.0 unx    16604 b- defN 24-Apr-03 21:38 determined/core/_distributed.py
+-rw-r--r--  2.0 unx     2884 b- defN 24-Apr-03 21:38 determined/core/_experimental.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-Apr-03 21:38 determined/core/_heartbeat.py
+-rw-r--r--  2.0 unx     5680 b- defN 24-Apr-03 21:38 determined/core/_log_shipper.py
+-rw-r--r--  2.0 unx    12734 b- defN 24-Apr-03 21:38 determined/core/_preempt.py
+-rw-r--r--  2.0 unx    17194 b- defN 24-Apr-03 21:38 determined/core/_profiler.py
+-rw-r--r--  2.0 unx    15041 b- defN 24-Apr-03 21:38 determined/core/_searcher.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-03 21:38 determined/core/_tensorboard_mode.py
+-rw-r--r--  2.0 unx    12099 b- defN 24-Apr-03 21:38 determined/core/_train.py
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-03 21:38 determined/deploy/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-03 21:38 determined/deploy/cli.py
+-rw-r--r--  2.0 unx      855 b- defN 24-Apr-03 21:38 determined/deploy/errors.py
+-rw-r--r--  2.0 unx     2109 b- defN 24-Apr-03 21:38 determined/deploy/healthcheck.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/aws/__init__.py
+-rw-r--r--  2.0 unx    19768 b- defN 24-Apr-03 21:38 determined/deploy/aws/aws.py
+-rw-r--r--  2.0 unx    29160 b- defN 24-Apr-03 21:38 determined/deploy/aws/cli.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-Apr-03 21:38 determined/deploy/aws/constants.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-03 21:38 determined/deploy/aws/gen_vcpu_mapping.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-Apr-03 21:38 determined/deploy/aws/master_config_inject.py
+-rw-r--r--  2.0 unx     5193 b- defN 24-Apr-03 21:38 determined/deploy/aws/preflight.py
+-rw-r--r--  2.0 unx    17324 b- defN 24-Apr-03 21:38 determined/deploy/aws/vcpu_mapping.yaml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/__init__.py
+-rw-r--r--  2.0 unx     5961 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/base.py
+-rw-r--r--  2.0 unx     1593 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/govcloud.py
+-rw-r--r--  2.0 unx     3094 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/secure.py
+-rw-r--r--  2.0 unx     1886 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/simple.py
+-rw-r--r--  2.0 unx     2381 b- defN 24-Apr-03 21:38 determined/deploy/aws/deployment_types/vpc.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/__init__.py
+-rw-r--r--  2.0 unx    30153 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/efs.yaml
+-rw-r--r--  2.0 unx    30863 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/fsx.yaml
+-rw-r--r--  2.0 unx    24489 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/govcloud.yaml
+-rw-r--r--  2.0 unx    32137 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/lore.yaml
+-rw-r--r--  2.0 unx    30025 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/secure.yaml
+-rw-r--r--  2.0 unx    26082 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/simple-rds.yaml
+-rw-r--r--  2.0 unx    25798 b- defN 24-Apr-03 21:38 determined/deploy/aws/templates/simple.yaml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/gcp/__init__.py
+-rw-r--r--  2.0 unx    25487 b- defN 24-Apr-03 21:38 determined/deploy/gcp/cli.py
+-rw-r--r--  2.0 unx      771 b- defN 24-Apr-03 21:38 determined/deploy/gcp/constants.py
+-rw-r--r--  2.0 unx    15099 b- defN 24-Apr-03 21:38 determined/deploy/gcp/gcp.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-Apr-03 21:38 determined/deploy/gcp/preflight.py
+-rw-r--r--  2.0 unx     5428 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/main.tf
+-rw-r--r--  2.0 unx     1647 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/master.yaml.tmpl
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/outputs.tf
+-rw-r--r--  2.0 unx     3836 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/variables.tf
+-rw-r--r--  2.0 unx     6195 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/compute/main.tf
+-rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/compute/outputs.tf
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/compute/variables.tf
+-rw-r--r--  2.0 unx     1222 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/database/main.tf
+-rw-r--r--  2.0 unx      283 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/database/outputs.tf
+-rw-r--r--  2.0 unx      320 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/database/variables.tf
+-rw-r--r--  2.0 unx      522 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/filestore/main.tf
+-rw-r--r--  2.0 unx      184 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
+-rw-r--r--  2.0 unx      125 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/filestore/variables.tf
+-rw-r--r--  2.0 unx     1026 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/firewall/main.tf
+-rw-r--r--  2.0 unx      195 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
+-rw-r--r--  2.0 unx       75 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/firewall/variables.tf
+-rw-r--r--  2.0 unx      637 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/gcs/main.tf
+-rw-r--r--  2.0 unx       51 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/gcs/variables.tf
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/ip/main.tf
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/ip/outputs.tf
+-rw-r--r--  2.0 unx       88 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/ip/variables.tf
+-rw-r--r--  2.0 unx     1112 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/network/main.tf
+-rw-r--r--  2.0 unx      275 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/network/outputs.tf
+-rw-r--r--  2.0 unx      207 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/network/variables.tf
+-rw-r--r--  2.0 unx      962 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/service_account/main.tf
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-03 21:38 determined/deploy/gcp/terraform/modules/service_account/variables.tf
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/gke/__init__.py
+-rw-r--r--  2.0 unx    19671 b- defN 24-Apr-03 21:38 determined/deploy/gke/cli.py
+-rw-r--r--  2.0 unx      408 b- defN 24-Apr-03 21:38 determined/deploy/gke/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/deploy/local/__init__.py
+-rw-r--r--  2.0 unx    13137 b- defN 24-Apr-03 21:38 determined/deploy/local/cli.py
+-rw-r--r--  2.0 unx    17119 b- defN 24-Apr-03 21:38 determined/deploy/local/cluster_utils.py
+-rw-r--r--  2.0 unx     1134 b- defN 24-Apr-03 21:38 determined/deploy/local/preflight.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/exec/__init__.py
+-rw-r--r--  2.0 unx     5473 b- defN 24-Apr-03 21:38 determined/exec/gc_checkpoints.py
+-rw-r--r--  2.0 unx     8475 b- defN 24-Apr-03 21:38 determined/exec/harness.py
+-rw-r--r--  2.0 unx     3695 b- defN 24-Apr-03 21:38 determined/exec/launch.py
+-rw-r--r--  2.0 unx      389 b- defN 24-Apr-03 21:38 determined/exec/pid_client.py
+-rw-r--r--  2.0 unx     1718 b- defN 24-Apr-03 21:38 determined/exec/pid_server.py
+-rw-r--r--  2.0 unx    13760 b- defN 24-Apr-03 21:38 determined/exec/prep_container.py
+-rw-r--r--  2.0 unx    11234 b- defN 24-Apr-03 21:38 determined/exec/tensorboard.py
+-rw-r--r--  2.0 unx      611 b- defN 24-Apr-03 21:38 determined/experimental/__init__.py
+-rw-r--r--  2.0 unx     3536 b- defN 24-Apr-03 21:38 determined/experimental/_native.py
+-rw-r--r--  2.0 unx    22391 b- defN 24-Apr-03 21:38 determined/experimental/client.py
+-rw-r--r--  2.0 unx      959 b- defN 24-Apr-03 21:38 determined/experimental/core_v2/__init__.py
+-rw-r--r--  2.0 unx     6260 b- defN 24-Apr-03 21:38 determined/experimental/core_v2/_core_context_v2.py
+-rw-r--r--  2.0 unx     8851 b- defN 24-Apr-03 21:38 determined/experimental/core_v2/_core_v2.py
+-rw-r--r--  2.0 unx     9851 b- defN 24-Apr-03 21:38 determined/experimental/core_v2/_unmanaged.py
+-rw-r--r--  2.0 unx      744 b- defN 24-Apr-03 21:38 determined/keras/__init__.py
+-rw-r--r--  2.0 unx     7579 b- defN 24-Apr-03 21:38 determined/keras/_data.py
+-rw-r--r--  2.0 unx    11491 b- defN 24-Apr-03 21:38 determined/keras/_enqueuer.py
+-rw-r--r--  2.0 unx     4066 b- defN 24-Apr-03 21:38 determined/keras/_load.py
+-rw-r--r--  2.0 unx      533 b- defN 24-Apr-03 21:38 determined/keras/_tensorboard_callback.py
+-rw-r--r--  2.0 unx    19081 b- defN 24-Apr-03 21:38 determined/keras/_tf_keras_context.py
+-rw-r--r--  2.0 unx     1251 b- defN 24-Apr-03 21:38 determined/keras/_tf_keras_multi_gpu.py
+-rw-r--r--  2.0 unx    47995 b- defN 24-Apr-03 21:38 determined/keras/_tf_keras_trial.py
+-rw-r--r--  2.0 unx    27517 b- defN 24-Apr-03 21:38 determined/keras/callbacks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/launch/__init__.py
+-rw-r--r--  2.0 unx    15109 b- defN 24-Apr-03 21:38 determined/launch/deepspeed.py
+-rw-r--r--  2.0 unx    10780 b- defN 24-Apr-03 21:38 determined/launch/horovod.py
+-rw-r--r--  2.0 unx     4640 b- defN 24-Apr-03 21:38 determined/launch/torch_distributed.py
+-rw-r--r--  2.0 unx     6831 b- defN 24-Apr-03 21:38 determined/launch/wrap_rank.py
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-03 21:38 determined/layers/__init__.py
+-rw-r--r--  2.0 unx    19697 b- defN 24-Apr-03 21:38 determined/layers/_workload_sequencer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 21:38 determined/lightning/__init__.py
+-rw-r--r--  2.0 unx     1847 b- defN 24-Apr-03 21:38 determined/lightning/experimental.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-03 21:38 determined/pytorch/__init__.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-03 21:38 determined/pytorch/_callback.py
+-rw-r--r--  2.0 unx    16717 b- defN 24-Apr-03 21:38 determined/pytorch/_data.py
+-rw-r--r--  2.0 unx     3716 b- defN 24-Apr-03 21:38 determined/pytorch/_experimental.py
+-rw-r--r--  2.0 unx    12557 b- defN 24-Apr-03 21:38 determined/pytorch/_load.py
+-rw-r--r--  2.0 unx     3286 b- defN 24-Apr-03 21:38 determined/pytorch/_lr_scheduler.py
+-rw-r--r--  2.0 unx     8322 b- defN 24-Apr-03 21:38 determined/pytorch/_metric_utils.py
+-rw-r--r--  2.0 unx    46422 b- defN 24-Apr-03 21:38 determined/pytorch/_pytorch_context.py
+-rw-r--r--  2.0 unx    68495 b- defN 24-Apr-03 21:38 determined/pytorch/_pytorch_trial.py
+-rw-r--r--  2.0 unx    21628 b- defN 24-Apr-03 21:38 determined/pytorch/_reducer.py
+-rw-r--r--  2.0 unx    14449 b- defN 24-Apr-03 21:38 determined/pytorch/_trainer.py
+-rw-r--r--  2.0 unx     9561 b- defN 24-Apr-03 21:38 determined/pytorch/samplers.py
+-rw-r--r--  2.0 unx      347 b- defN 24-Apr-03 21:38 determined/pytorch/deepspeed/__init__.py
+-rw-r--r--  2.0 unx    19896 b- defN 24-Apr-03 21:38 determined/pytorch/deepspeed/_deepspeed_context.py
+-rw-r--r--  2.0 unx    43012 b- defN 24-Apr-03 21:38 determined/pytorch/deepspeed/_deepspeed_trial.py
+-rw-r--r--  2.0 unx     1987 b- defN 24-Apr-03 21:38 determined/pytorch/deepspeed/_mpu.py
+-rw-r--r--  2.0 unx      409 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/__main__.py
+-rw-r--r--  2.0 unx     2541 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/_defaults.py
+-rw-r--r--  2.0 unx    60179 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/_dsat_search_method.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/_run_dsat.py
+-rw-r--r--  2.0 unx    20150 b- defN 24-Apr-03 21:38 determined/pytorch/dsat/_utils.py
+-rw-r--r--  2.0 unx      175 b- defN 24-Apr-03 21:38 determined/pytorch/experimental/__init__.py
+-rw-r--r--  2.0 unx    21611 b- defN 24-Apr-03 21:38 determined/pytorch/experimental/_torch_batch_process.py
+-rw-r--r--  2.0 unx      343 b- defN 24-Apr-03 21:38 determined/searcher/__init__.py
+-rw-r--r--  2.0 unx     4134 b- defN 24-Apr-03 21:38 determined/searcher/_remote_search_runner.py
+-rw-r--r--  2.0 unx    16436 b- defN 24-Apr-03 21:38 determined/searcher/_search_method.py
+-rw-r--r--  2.0 unx    15961 b- defN 24-Apr-03 21:38 determined/searcher/_search_runner.py
+-rw-r--r--  2.0 unx      512 b- defN 24-Apr-03 21:38 determined/tensorboard/__init__.py
+-rw-r--r--  2.0 unx     1579 b- defN 24-Apr-03 21:38 determined/tensorboard/azure.py
+-rw-r--r--  2.0 unx     6111 b- defN 24-Apr-03 21:38 determined/tensorboard/base.py
+-rw-r--r--  2.0 unx     4641 b- defN 24-Apr-03 21:38 determined/tensorboard/build.py
+-rw-r--r--  2.0 unx      225 b- defN 24-Apr-03 21:38 determined/tensorboard/directory.py
+-rw-r--r--  2.0 unx     2357 b- defN 24-Apr-03 21:38 determined/tensorboard/gcs.py
+-rw-r--r--  2.0 unx     1895 b- defN 24-Apr-03 21:38 determined/tensorboard/s3.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-03 21:38 determined/tensorboard/shared.py
+-rw-r--r--  2.0 unx     3787 b- defN 24-Apr-03 21:38 determined/tensorboard/util.py
+-rw-r--r--  2.0 unx      845 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/__init__.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/azure.py
+-rw-r--r--  2.0 unx     1670 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/base.py
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/directory.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/gcs.py
+-rw-r--r--  2.0 unx     2495 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/s3.py
+-rw-r--r--  2.0 unx     1657 b- defN 24-Apr-03 21:38 determined/tensorboard/fetchers/shared.py
+-rw-r--r--  2.0 unx       91 b- defN 24-Apr-03 21:38 determined/tensorboard/metric_writers/__init__.py
+-rw-r--r--  2.0 unx     3313 b- defN 24-Apr-03 21:38 determined/tensorboard/metric_writers/callback.py
+-rw-r--r--  2.0 unx     3255 b- defN 24-Apr-03 21:38 determined/tensorboard/metric_writers/pytorch.py
+-rw-r--r--  2.0 unx     4443 b- defN 24-Apr-03 21:38 determined/tensorboard/metric_writers/tensorflow.py
+-rw-r--r--  2.0 unx       70 b- defN 24-Apr-03 21:38 determined/transformers/__init__.py
+-rw-r--r--  2.0 unx    12730 b- defN 24-Apr-03 21:38 determined/transformers/_hf_callback.py
+-rw-r--r--  2.0 unx     1242 b- defN 24-Apr-03 21:39 determined-0.30.0rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 21:39 determined-0.30.0rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-03 21:39 determined-0.30.0rc5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-03 21:39 determined-0.30.0rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    24976 b- defN 24-Apr-03 21:39 determined-0.30.0rc5.dist-info/RECORD
+271 files, 2880438 bytes uncompressed, 641384 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -792,23 +792,23 @@
 
 Filename: determined/transformers/__init__.py
 Comment: 
 
 Filename: determined/transformers/_hf_callback.py
 Comment: 
 
-Filename: determined-0.30.0rc4.dist-info/METADATA
+Filename: determined-0.30.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: determined-0.30.0rc4.dist-info/WHEEL
+Filename: determined-0.30.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: determined-0.30.0rc4.dist-info/entry_points.txt
+Filename: determined-0.30.0rc5.dist-info/entry_points.txt
 Comment: 
 
-Filename: determined-0.30.0rc4.dist-info/top_level.txt
+Filename: determined-0.30.0rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: determined-0.30.0rc4.dist-info/RECORD
+Filename: determined-0.30.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.30.0-rc4"
+__version__ = "0.30.0-rc5"
```

## determined/deploy/aws/templates/efs.yaml

```diff
@@ -97,15 +97,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## determined/deploy/aws/templates/fsx.yaml

```diff
@@ -97,15 +97,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## determined/deploy/aws/templates/govcloud.yaml

```diff
@@ -63,15 +63,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master docker image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## determined/deploy/aws/templates/lore.yaml

```diff
@@ -97,15 +97,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## determined/deploy/aws/templates/secure.yaml

```diff
@@ -118,15 +118,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## determined/deploy/aws/templates/simple-rds.yaml

```diff
@@ -89,15 +89,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master docker image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   DBInstanceType:
```

## determined/deploy/aws/templates/simple.yaml

```diff
@@ -89,15 +89,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master docker image
-    Default: 0.30.0-rc4
+    Default: 0.30.0-rc5
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## Comparing `determined-0.30.0rc4.dist-info/METADATA` & `determined-0.30.0rc5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: determined
-Version: 0.30.0rc4
+Version: 0.30.0rc5
 Summary: Determined Deep Learning Training Platform
 Home-page: https://determined.ai/
 Author: Determined AI
 Author-email: hello@determined.ai
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
```

## Comparing `determined-0.30.0rc4.dist-info/RECORD` & `determined-0.30.0rc5.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 determined/__init__.py,sha256=AylNLk96_lQOsbYJsIZYy-p9ElH-1qhuwRWvkNXqAtc,1140
-determined/__version__.py,sha256=bpNALqy9KcqicDg3eHoG820qpX91I2Ev892ExQNiJsg,27
+determined/__version__.py,sha256=jTP7WrVZU6xW4S96ZC45OjEBzEnargXRjTJjnj52P7E,27
 determined/_env_context.py,sha256=vG1rREr-gp-rVjGUn_5mzKhRxC8qv0RwpNY4rABT_h4,1664
 determined/_execution.py,sha256=FciLz0KifU2uxiZTOgDmuTTPyQj_mKeX90qNiU0IMS8,8854
 determined/_experiment_config.py,sha256=kkHvFHQzkI3HlckUozKwjfaieWIgeEot9jyPtvQuLjs,2779
 determined/_import.py,sha256=czaz1MQU8w2tfkeD3rIAVDpRyS_7lH0K9Sn-_zm2luQ,4781
 determined/_info.py,sha256=tc3R_0hwIRGRU7gx-lj4tLVbjjKJiZuQFGDkWBEwKCI,14970
 determined/_tf_rng.py,sha256=Z96_dEFOB2BRWyrthYN1A2FKxGe-fi0XKS_AEupLAnM,1272
 determined/_trial.py,sha256=7OagQh74mwD2FY6VHWTsKH6kiZIBrF_318gqRtcbtvc,1220
@@ -130,21 +130,21 @@
 determined/deploy/aws/deployment_types/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/aws/deployment_types/base.py,sha256=7zdGEqjTCJYMa_hsDBg899A_GclOvR_4tzDTS3fMUsA,5961
 determined/deploy/aws/deployment_types/govcloud.py,sha256=BjLMhQy9QreojfjBacO2Lg-g-fIVvq4cSDQc_HsDDC4,1593
 determined/deploy/aws/deployment_types/secure.py,sha256=E-EHO1PnlZoi4dXf17PLhSE18ceRjPklTf__2PsHGgQ,3094
 determined/deploy/aws/deployment_types/simple.py,sha256=YJF8j4ALnwTSkE531MlxFC1ZZLlAVEsfsIescV_XJ4k,1886
 determined/deploy/aws/deployment_types/vpc.py,sha256=zU0ouLlRXs4kHrCPSQO85xnV4Y7wCKT9anjNNmnGW2M,2381
 determined/deploy/aws/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-determined/deploy/aws/templates/efs.yaml,sha256=JXbz38XJvIXFSeWMkwKi_VITkPBuIYom-NER0xFvVak,30153
-determined/deploy/aws/templates/fsx.yaml,sha256=WU6IywAygPLFKeol4fo-hxH2qTvCAHZe8U8USygRvHI,30863
-determined/deploy/aws/templates/govcloud.yaml,sha256=ZbP41m8GHsmLQXd89ccpyPflo7hSPQH4Rrcs1kgJiF0,24489
-determined/deploy/aws/templates/lore.yaml,sha256=GFSXwWbL8AGo71_Bg7Uw5R8e36A0lE7tdrMwHDceZ9k,32137
-determined/deploy/aws/templates/secure.yaml,sha256=MQQ_b9fW2lqpYJi1q7PD8ml21vD4dOH5abCYjugnhck,30025
-determined/deploy/aws/templates/simple-rds.yaml,sha256=yA0NIh75808z_J5L8dg6WZgm9EZnO7WiWsZVLxFglT4,26082
-determined/deploy/aws/templates/simple.yaml,sha256=ByfkiE5uwR6o7udZXJXAcU4Jay_HNUQRzkNECHGASOM,25798
+determined/deploy/aws/templates/efs.yaml,sha256=4hqU1S8FSSUelmCVx9LP3JgCjIDGYj_nignXa7nsvDE,30153
+determined/deploy/aws/templates/fsx.yaml,sha256=t5d90CK5mtr1lEbX0z48IO8c7il352ypBW6mC9RDgYg,30863
+determined/deploy/aws/templates/govcloud.yaml,sha256=vP8FrlboXpkNXLnGkG6gn7gY-O85Vfr6dPl_X1TYwx8,24489
+determined/deploy/aws/templates/lore.yaml,sha256=Yo0qg3Qde75ACj1to_d4G17HbnoO6A8uYWDIJ-bYw0s,32137
+determined/deploy/aws/templates/secure.yaml,sha256=yUikWYAd7HFbIJRG1pOyE47vOLcKoVv2Lwqbhxx87SA,30025
+determined/deploy/aws/templates/simple-rds.yaml,sha256=xv0mmwgyI5CRnUnCsiq_do8UZR-j2pa_rjpDlWTuZcU,26082
+determined/deploy/aws/templates/simple.yaml,sha256=1SThJDQhlxzpuWj0gXrVsrP3SNZ6QWAfcJzt3BhErgI,25798
 determined/deploy/gcp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/gcp/cli.py,sha256=LqiDMHLgJHKosoZd7UMlMZJQPdIpMsxvbabXBVc3QSc,25487
 determined/deploy/gcp/constants.py,sha256=WFNy7xR4GywyJz7hTt97IoY0rR87ucl4oWL1aK6TEvY,771
 determined/deploy/gcp/gcp.py,sha256=-5IrW4LLePPiYZxYC3MUBFP_n-F2tbkb9IQKPPcdofs,15099
 determined/deploy/gcp/preflight.py,sha256=LdZ9IimNp_79YxEit8_MIlH7uTnzKvnBF8hlOphlyfA,2464
 determined/deploy/gcp/terraform/main.tf,sha256=x7gr1uL09albo6w0hFIe-09XC49rpz5UqiTDmQn2Qo4,5428
 determined/deploy/gcp/terraform/master.yaml.tmpl,sha256=D29nT4FTVAakjqaa_Ca8b2jim4LE_9EYOH00Ji4yvbE,1647
@@ -260,12 +260,12 @@
 determined/tensorboard/fetchers/shared.py,sha256=RKMfKTw9ILZwKps-sgoDz6aKcw1bFBbBiSvAzLOfF7k,1657
 determined/tensorboard/metric_writers/__init__.py,sha256=QBZlDYJslTPnllbOOwzbV_XtKlsLwf9SR8YcL3MdJtY,91
 determined/tensorboard/metric_writers/callback.py,sha256=tmw-nFAe6uAhnEBL29LyjTf4chzOfhg2RIo2ANYm4Rw,3313
 determined/tensorboard/metric_writers/pytorch.py,sha256=J8dyqXIfzsSjtFj649noxwTx3cOxGanQ6c-Q1Aya7Cc,3255
 determined/tensorboard/metric_writers/tensorflow.py,sha256=fPWjvDmnNl-xEpVnDh0BEfffi4n21ttL-FPDEe2BSbE,4443
 determined/transformers/__init__.py,sha256=WJSvfLUkyIXjrbAKEe-SRXYdl8ZuDceqztiZ0ASJKIA,70
 determined/transformers/_hf_callback.py,sha256=dPi6cTE2fGraUuxqAADVEYQrv6hiRDSv9KQv08XxzCQ,12730
-determined-0.30.0rc4.dist-info/METADATA,sha256=q_mgsrUZDorxhVuDX9hSFNtXMIVcfIZApXl8xpiQT24,1242
-determined-0.30.0rc4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-determined-0.30.0rc4.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
-determined-0.30.0rc4.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
-determined-0.30.0rc4.dist-info/RECORD,,
+determined-0.30.0rc5.dist-info/METADATA,sha256=FcbfxCQKxGWi98LZRGRKc85uz7R_84VvSTPldXGuutM,1242
+determined-0.30.0rc5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+determined-0.30.0rc5.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
+determined-0.30.0rc5.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
+determined-0.30.0rc5.dist-info/RECORD,,
```

