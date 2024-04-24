# Comparing `tmp/determined-0.31.1rc0-py3-none-any.whl.zip` & `tmp/determined-0.32.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,275 +1,275 @@
-Zip file size: 689297 bytes, number of entries: 273
--rw-r--r--  2.0 unx     1140 b- defN 24-Apr-24 00:28 determined/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 24-Apr-24 00:28 determined/__version__.py
--rw-r--r--  2.0 unx     1664 b- defN 24-Apr-24 00:28 determined/_env_context.py
--rw-r--r--  2.0 unx     8854 b- defN 24-Apr-24 00:28 determined/_execution.py
--rw-r--r--  2.0 unx     2779 b- defN 24-Apr-24 00:28 determined/_experiment_config.py
--rw-r--r--  2.0 unx     4781 b- defN 24-Apr-24 00:28 determined/_import.py
--rw-r--r--  2.0 unx    14970 b- defN 24-Apr-24 00:28 determined/_info.py
--rw-r--r--  2.0 unx     1220 b- defN 24-Apr-24 00:28 determined/_trial.py
--rw-r--r--  2.0 unx     4777 b- defN 24-Apr-24 00:28 determined/_trial_context.py
--rw-r--r--  2.0 unx     3246 b- defN 24-Apr-24 00:28 determined/_trial_controller.py
--rw-r--r--  2.0 unx     2271 b- defN 24-Apr-24 00:28 determined/constants.py
--rw-r--r--  2.0 unx     2734 b- defN 24-Apr-24 00:28 determined/errors.py
--rw-r--r--  2.0 unx     5627 b- defN 24-Apr-24 00:28 determined/gpu.py
--rw-r--r--  2.0 unx     6182 b- defN 24-Apr-24 00:28 determined/horovod.py
--rw-r--r--  2.0 unx    20027 b- defN 24-Apr-24 00:28 determined/ipc.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-24 00:28 determined/load.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/py.typed
--rw-r--r--  2.0 unx    18236 b- defN 24-Apr-24 00:28 determined/util.py
--rw-r--r--  2.0 unx     6570 b- defN 24-Apr-24 00:28 determined/workload.py
--rw-r--r--  2.0 unx      805 b- defN 24-Apr-24 00:28 determined/cli/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 24-Apr-24 00:28 determined/cli/__main__.py
--rw-r--r--  2.0 unx     8425 b- defN 24-Apr-24 00:28 determined/cli/_declarative_argparse.py
--rw-r--r--  2.0 unx     3968 b- defN 24-Apr-24 00:28 determined/cli/_util.py
--rw-r--r--  2.0 unx    10013 b- defN 24-Apr-24 00:28 determined/cli/agent.py
--rw-r--r--  2.0 unx     8306 b- defN 24-Apr-24 00:28 determined/cli/checkpoint.py
--rw-r--r--  2.0 unx    10483 b- defN 24-Apr-24 00:28 determined/cli/cli.py
--rw-r--r--  2.0 unx     5252 b- defN 24-Apr-24 00:28 determined/cli/command.py
--rw-r--r--  2.0 unx    11680 b- defN 24-Apr-24 00:28 determined/cli/dev.py
--rw-r--r--  2.0 unx      627 b- defN 24-Apr-24 00:28 determined/cli/errors.py
--rw-r--r--  2.0 unx    52218 b- defN 24-Apr-24 00:28 determined/cli/experiment.py
--rw-r--r--  2.0 unx     8714 b- defN 24-Apr-24 00:28 determined/cli/job.py
--rw-r--r--  2.0 unx     4595 b- defN 24-Apr-24 00:28 determined/cli/master.py
--rw-r--r--  2.0 unx     8479 b- defN 24-Apr-24 00:28 determined/cli/model.py
--rw-r--r--  2.0 unx     7104 b- defN 24-Apr-24 00:28 determined/cli/notebook.py
--rw-r--r--  2.0 unx    16661 b- defN 24-Apr-24 00:28 determined/cli/ntsc.py
--rw-r--r--  2.0 unx     1870 b- defN 24-Apr-24 00:28 determined/cli/oauth.py
--rw-r--r--  2.0 unx    11874 b- defN 24-Apr-24 00:28 determined/cli/project.py
--rw-r--r--  2.0 unx     7918 b- defN 24-Apr-24 00:28 determined/cli/proxy.py
--rw-r--r--  2.0 unx    18598 b- defN 24-Apr-24 00:28 determined/cli/rbac.py
--rw-r--r--  2.0 unx    10204 b- defN 24-Apr-24 00:28 determined/cli/render.py
--rw-r--r--  2.0 unx     5199 b- defN 24-Apr-24 00:28 determined/cli/resource_pool.py
--rw-r--r--  2.0 unx     2282 b- defN 24-Apr-24 00:28 determined/cli/resources.py
--rw-r--r--  2.0 unx    13213 b- defN 24-Apr-24 00:28 determined/cli/shell.py
--rw-r--r--  2.0 unx     5136 b- defN 24-Apr-24 00:28 determined/cli/sso.py
--rw-r--r--  2.0 unx    13307 b- defN 24-Apr-24 00:28 determined/cli/task.py
--rw-r--r--  2.0 unx     5300 b- defN 24-Apr-24 00:28 determined/cli/template.py
--rw-r--r--  2.0 unx     7638 b- defN 24-Apr-24 00:28 determined/cli/tensorboard.py
--rw-r--r--  2.0 unx      111 b- defN 24-Apr-24 00:28 determined/cli/top_arg_descriptions.py
--rw-r--r--  2.0 unx    19091 b- defN 24-Apr-24 00:28 determined/cli/trial.py
--rw-r--r--  2.0 unx     1635 b- defN 24-Apr-24 00:28 determined/cli/tunnel.py
--rw-r--r--  2.0 unx    11091 b- defN 24-Apr-24 00:28 determined/cli/user.py
--rw-r--r--  2.0 unx     8373 b- defN 24-Apr-24 00:28 determined/cli/user_groups.py
--rw-r--r--  2.0 unx     2526 b- defN 24-Apr-24 00:28 determined/cli/version.py
--rw-r--r--  2.0 unx    15325 b- defN 24-Apr-24 00:28 determined/cli/workspace.py
--rw-r--r--  2.0 unx      352 b- defN 24-Apr-24 00:28 determined/common/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-24 00:28 determined/common/_logging.py
--rw-r--r--  2.0 unx     8593 b- defN 24-Apr-24 00:28 determined/common/check.py
--rw-r--r--  2.0 unx     2154 b- defN 24-Apr-24 00:28 determined/common/constants.py
--rw-r--r--  2.0 unx     4278 b- defN 24-Apr-24 00:28 determined/common/context.py
--rw-r--r--  2.0 unx     3569 b- defN 24-Apr-24 00:28 determined/common/detignore.py
--rw-r--r--  2.0 unx     3328 b- defN 24-Apr-24 00:28 determined/common/detlomond.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/common/py.typed
--rw-r--r--  2.0 unx     1662 b- defN 24-Apr-24 00:28 determined/common/requests.py
--rw-r--r--  2.0 unx    11922 b- defN 24-Apr-24 00:28 determined/common/util.py
--rw-r--r--  2.0 unx     1516 b- defN 24-Apr-24 00:28 determined/common/v1file_utils.py
--rw-r--r--  2.0 unx      809 b- defN 24-Apr-24 00:28 determined/common/api/__init__.py
--rw-r--r--  2.0 unx     4219 b- defN 24-Apr-24 00:28 determined/common/api/_rbac.py
--rw-r--r--  2.0 unx     8891 b- defN 24-Apr-24 00:28 determined/common/api/_session.py
--rw-r--r--  2.0 unx     6288 b- defN 24-Apr-24 00:28 determined/common/api/_util.py
--rw-r--r--  2.0 unx     1469 b- defN 24-Apr-24 00:28 determined/common/api/analytics.py
--rw-r--r--  2.0 unx    23171 b- defN 24-Apr-24 00:28 determined/common/api/authentication.py
--rw-r--r--  2.0 unx   828044 b- defN 24-Apr-24 00:28 determined/common/api/bindings.py
--rw-r--r--  2.0 unx     7421 b- defN 24-Apr-24 00:28 determined/common/api/certs.py
--rw-r--r--  2.0 unx     4010 b- defN 24-Apr-24 00:28 determined/common/api/errors.py
--rw-r--r--  2.0 unx     3281 b- defN 24-Apr-24 00:28 determined/common/api/logs.py
--rw-r--r--  2.0 unx      247 b- defN 24-Apr-24 00:28 determined/common/api/metric.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-24 00:28 determined/common/experimental/__init__.py
--rw-r--r--  2.0 unx      465 b- defN 24-Apr-24 00:28 determined/common/experimental/_util.py
--rw-r--r--  2.0 unx    23950 b- defN 24-Apr-24 00:28 determined/common/experimental/determined.py
--rw-r--r--  2.0 unx    26924 b- defN 24-Apr-24 00:28 determined/common/experimental/experiment.py
--rw-r--r--  2.0 unx     3567 b- defN 24-Apr-24 00:28 determined/common/experimental/metrics.py
--rw-r--r--  2.0 unx    16083 b- defN 24-Apr-24 00:28 determined/common/experimental/model.py
--rw-r--r--  2.0 unx      306 b- defN 24-Apr-24 00:28 determined/common/experimental/oauth2_scim_client.py
--rw-r--r--  2.0 unx     7712 b- defN 24-Apr-24 00:28 determined/common/experimental/project.py
--rw-r--r--  2.0 unx     3607 b- defN 24-Apr-24 00:28 determined/common/experimental/resource_pool.py
--rw-r--r--  2.0 unx    25650 b- defN 24-Apr-24 00:28 determined/common/experimental/trial.py
--rw-r--r--  2.0 unx     5056 b- defN 24-Apr-24 00:28 determined/common/experimental/user.py
--rw-r--r--  2.0 unx     5801 b- defN 24-Apr-24 00:28 determined/common/experimental/workspace.py
--rw-r--r--  2.0 unx      170 b- defN 24-Apr-24 00:28 determined/common/experimental/checkpoint/__init__.py
--rw-r--r--  2.0 unx    20350 b- defN 24-Apr-24 00:28 determined/common/experimental/checkpoint/_checkpoint.py
--rw-r--r--  2.0 unx     4182 b- defN 24-Apr-24 00:28 determined/common/storage/__init__.py
--rw-r--r--  2.0 unx      479 b- defN 24-Apr-24 00:28 determined/common/storage/_util.py
--rw-r--r--  2.0 unx     4339 b- defN 24-Apr-24 00:28 determined/common/storage/azure.py
--rw-r--r--  2.0 unx     3638 b- defN 24-Apr-24 00:28 determined/common/storage/azure_client.py
--rw-r--r--  2.0 unx     9368 b- defN 24-Apr-24 00:28 determined/common/storage/base.py
--rw-r--r--  2.0 unx     4445 b- defN 24-Apr-24 00:28 determined/common/storage/boto3_credential_manager.py
--rw-r--r--  2.0 unx     1014 b- defN 24-Apr-24 00:28 determined/common/storage/cloud.py
--rw-r--r--  2.0 unx     2282 b- defN 24-Apr-24 00:28 determined/common/storage/directory.py
--rw-r--r--  2.0 unx     6479 b- defN 24-Apr-24 00:28 determined/common/storage/gcs.py
--rw-r--r--  2.0 unx     6269 b- defN 24-Apr-24 00:28 determined/common/storage/s3.py
--rw-r--r--  2.0 unx     9868 b- defN 24-Apr-24 00:28 determined/common/storage/shared.py
--rw-r--r--  2.0 unx      243 b- defN 24-Apr-24 00:28 determined/common/streams/__init__.py
--rw-r--r--  2.0 unx    19565 b- defN 24-Apr-24 00:28 determined/common/streams/_client.py
--rw-r--r--  2.0 unx      391 b- defN 24-Apr-24 00:28 determined/common/streams/_util.py
--rw-r--r--  2.0 unx     5357 b- defN 24-Apr-24 00:28 determined/common/streams/wire.py
--rw-r--r--  2.0 unx     1405 b- defN 24-Apr-24 00:28 determined/core/__init__.py
--rw-r--r--  2.0 unx    30354 b- defN 24-Apr-24 00:28 determined/core/_checkpoint.py
--rw-r--r--  2.0 unx    14337 b- defN 24-Apr-24 00:28 determined/core/_context.py
--rw-r--r--  2.0 unx    16604 b- defN 24-Apr-24 00:28 determined/core/_distributed.py
--rw-r--r--  2.0 unx     2884 b- defN 24-Apr-24 00:28 determined/core/_experimental.py
--rw-r--r--  2.0 unx     4580 b- defN 24-Apr-24 00:28 determined/core/_heartbeat.py
--rw-r--r--  2.0 unx     5515 b- defN 24-Apr-24 00:28 determined/core/_log_shipper.py
--rw-r--r--  2.0 unx     6620 b- defN 24-Apr-24 00:28 determined/core/_metrics.py
--rw-r--r--  2.0 unx    12734 b- defN 24-Apr-24 00:28 determined/core/_preempt.py
--rw-r--r--  2.0 unx    14841 b- defN 24-Apr-24 00:28 determined/core/_profiler.py
--rw-r--r--  2.0 unx    15041 b- defN 24-Apr-24 00:28 determined/core/_searcher.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-24 00:28 determined/core/_tensorboard_mode.py
--rw-r--r--  2.0 unx    11806 b- defN 24-Apr-24 00:28 determined/core/_train.py
--rw-r--r--  2.0 unx       56 b- defN 24-Apr-24 00:28 determined/deploy/__init__.py
--rw-r--r--  2.0 unx      996 b- defN 24-Apr-24 00:28 determined/deploy/cli.py
--rw-r--r--  2.0 unx      855 b- defN 24-Apr-24 00:28 determined/deploy/errors.py
--rw-r--r--  2.0 unx     2109 b- defN 24-Apr-24 00:28 determined/deploy/healthcheck.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/aws/__init__.py
--rw-r--r--  2.0 unx    19820 b- defN 24-Apr-24 00:28 determined/deploy/aws/aws.py
--rw-r--r--  2.0 unx    29379 b- defN 24-Apr-24 00:28 determined/deploy/aws/cli.py
--rw-r--r--  2.0 unx     3322 b- defN 24-Apr-24 00:28 determined/deploy/aws/constants.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-24 00:28 determined/deploy/aws/gen_vcpu_mapping.py
--rw-r--r--  2.0 unx     2288 b- defN 24-Apr-24 00:28 determined/deploy/aws/master_config_inject.py
--rw-r--r--  2.0 unx     5234 b- defN 24-Apr-24 00:28 determined/deploy/aws/preflight.py
--rw-r--r--  2.0 unx    17324 b- defN 24-Apr-24 00:28 determined/deploy/aws/vcpu_mapping.yaml
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/__init__.py
--rw-r--r--  2.0 unx     6357 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/base.py
--rw-r--r--  2.0 unx     1590 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/govcloud.py
--rw-r--r--  2.0 unx     3131 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/secure.py
--rw-r--r--  2.0 unx     1886 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/simple.py
--rw-r--r--  2.0 unx     2381 b- defN 24-Apr-24 00:28 determined/deploy/aws/deployment_types/vpc.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/__init__.py
--rw-r--r--  2.0 unx    30197 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/efs.yaml
--rw-r--r--  2.0 unx    30907 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/fsx.yaml
--rw-r--r--  2.0 unx    24534 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/govcloud.yaml
--rw-r--r--  2.0 unx    32181 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/lore.yaml
--rw-r--r--  2.0 unx    30070 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/secure.yaml
--rw-r--r--  2.0 unx    26127 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/simple-rds.yaml
--rw-r--r--  2.0 unx    25843 b- defN 24-Apr-24 00:28 determined/deploy/aws/templates/simple.yaml
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/gcp/__init__.py
--rw-r--r--  2.0 unx    25639 b- defN 24-Apr-24 00:28 determined/deploy/gcp/cli.py
--rw-r--r--  2.0 unx      771 b- defN 24-Apr-24 00:28 determined/deploy/gcp/constants.py
--rw-r--r--  2.0 unx    15054 b- defN 24-Apr-24 00:28 determined/deploy/gcp/gcp.py
--rw-r--r--  2.0 unx     2494 b- defN 24-Apr-24 00:28 determined/deploy/gcp/preflight.py
--rw-r--r--  2.0 unx     5428 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/main.tf
--rw-r--r--  2.0 unx     1647 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/master.yaml.tmpl
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/outputs.tf
--rw-r--r--  2.0 unx     3836 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/variables.tf
--rw-r--r--  2.0 unx     6195 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/compute/main.tf
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/compute/outputs.tf
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/compute/variables.tf
--rw-r--r--  2.0 unx     1222 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/database/main.tf
--rw-r--r--  2.0 unx      283 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/database/outputs.tf
--rw-r--r--  2.0 unx      320 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/database/variables.tf
--rw-r--r--  2.0 unx      522 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/filestore/main.tf
--rw-r--r--  2.0 unx      184 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
--rw-r--r--  2.0 unx      125 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/filestore/variables.tf
--rw-r--r--  2.0 unx     1026 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/firewall/main.tf
--rw-r--r--  2.0 unx      195 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
--rw-r--r--  2.0 unx       75 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/firewall/variables.tf
--rw-r--r--  2.0 unx      637 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/gcs/main.tf
--rw-r--r--  2.0 unx       51 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
--rw-r--r--  2.0 unx      161 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/gcs/variables.tf
--rw-r--r--  2.0 unx      161 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/ip/main.tf
--rw-r--r--  2.0 unx      122 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/ip/outputs.tf
--rw-r--r--  2.0 unx       88 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/ip/variables.tf
--rw-r--r--  2.0 unx     1112 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/network/main.tf
--rw-r--r--  2.0 unx      275 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/network/outputs.tf
--rw-r--r--  2.0 unx      207 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/network/variables.tf
--rw-r--r--  2.0 unx      962 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/service_account/main.tf
--rw-r--r--  2.0 unx       73 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-24 00:28 determined/deploy/gcp/terraform/modules/service_account/variables.tf
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/gke/__init__.py
--rw-r--r--  2.0 unx    19788 b- defN 24-Apr-24 00:28 determined/deploy/gke/cli.py
--rw-r--r--  2.0 unx      408 b- defN 24-Apr-24 00:28 determined/deploy/gke/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/deploy/local/__init__.py
--rw-r--r--  2.0 unx    14111 b- defN 24-Apr-24 00:28 determined/deploy/local/cli.py
--rw-r--r--  2.0 unx    17552 b- defN 24-Apr-24 00:28 determined/deploy/local/cluster_utils.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-24 00:28 determined/deploy/local/preflight.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/exec/__init__.py
--rw-r--r--  2.0 unx     5473 b- defN 24-Apr-24 00:28 determined/exec/gc_checkpoints.py
--rw-r--r--  2.0 unx     8475 b- defN 24-Apr-24 00:28 determined/exec/harness.py
--rw-r--r--  2.0 unx     3695 b- defN 24-Apr-24 00:28 determined/exec/launch.py
--rw-r--r--  2.0 unx      389 b- defN 24-Apr-24 00:28 determined/exec/pid_client.py
--rw-r--r--  2.0 unx     1718 b- defN 24-Apr-24 00:28 determined/exec/pid_server.py
--rw-r--r--  2.0 unx    13760 b- defN 24-Apr-24 00:28 determined/exec/prep_container.py
--rw-r--r--  2.0 unx    11234 b- defN 24-Apr-24 00:28 determined/exec/tensorboard.py
--rw-r--r--  2.0 unx      611 b- defN 24-Apr-24 00:28 determined/experimental/__init__.py
--rw-r--r--  2.0 unx     3536 b- defN 24-Apr-24 00:28 determined/experimental/_native.py
--rw-r--r--  2.0 unx    23124 b- defN 24-Apr-24 00:28 determined/experimental/client.py
--rw-r--r--  2.0 unx      959 b- defN 24-Apr-24 00:28 determined/experimental/core_v2/__init__.py
--rw-r--r--  2.0 unx     6430 b- defN 24-Apr-24 00:28 determined/experimental/core_v2/_core_context_v2.py
--rw-r--r--  2.0 unx     8851 b- defN 24-Apr-24 00:28 determined/experimental/core_v2/_core_v2.py
--rw-r--r--  2.0 unx     9851 b- defN 24-Apr-24 00:28 determined/experimental/core_v2/_unmanaged.py
--rw-r--r--  2.0 unx      810 b- defN 24-Apr-24 00:28 determined/keras/__init__.py
--rw-r--r--  2.0 unx     7579 b- defN 24-Apr-24 00:28 determined/keras/_data.py
--rw-r--r--  2.0 unx    11491 b- defN 24-Apr-24 00:28 determined/keras/_enqueuer.py
--rw-r--r--  2.0 unx     4342 b- defN 24-Apr-24 00:28 determined/keras/_load.py
--rw-r--r--  2.0 unx      533 b- defN 24-Apr-24 00:28 determined/keras/_tensorboard_callback.py
--rw-r--r--  2.0 unx    19133 b- defN 24-Apr-24 00:28 determined/keras/_tf_keras_context.py
--rw-r--r--  2.0 unx     1251 b- defN 24-Apr-24 00:28 determined/keras/_tf_keras_multi_gpu.py
--rw-r--r--  2.0 unx    48227 b- defN 24-Apr-24 00:28 determined/keras/_tf_keras_trial.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-24 00:28 determined/keras/_tf_rng.py
--rw-r--r--  2.0 unx    27517 b- defN 24-Apr-24 00:28 determined/keras/callbacks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/launch/__init__.py
--rw-r--r--  2.0 unx    15061 b- defN 24-Apr-24 00:28 determined/launch/deepspeed.py
--rw-r--r--  2.0 unx    10762 b- defN 24-Apr-24 00:28 determined/launch/horovod.py
--rw-r--r--  2.0 unx     4640 b- defN 24-Apr-24 00:28 determined/launch/torch_distributed.py
--rw-r--r--  2.0 unx     6831 b- defN 24-Apr-24 00:28 determined/launch/wrap_rank.py
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 00:28 determined/layers/__init__.py
--rw-r--r--  2.0 unx    19697 b- defN 24-Apr-24 00:28 determined/layers/_workload_sequencer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 00:28 determined/lightning/__init__.py
--rw-r--r--  2.0 unx     1847 b- defN 24-Apr-24 00:28 determined/lightning/experimental.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-24 00:28 determined/pytorch/__init__.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-24 00:28 determined/pytorch/_callback.py
--rw-r--r--  2.0 unx    16640 b- defN 24-Apr-24 00:28 determined/pytorch/_data.py
--rw-r--r--  2.0 unx     3716 b- defN 24-Apr-24 00:28 determined/pytorch/_experimental.py
--rw-r--r--  2.0 unx    12557 b- defN 24-Apr-24 00:28 determined/pytorch/_load.py
--rw-r--r--  2.0 unx     3286 b- defN 24-Apr-24 00:28 determined/pytorch/_lr_scheduler.py
--rw-r--r--  2.0 unx     8322 b- defN 24-Apr-24 00:28 determined/pytorch/_metric_utils.py
--rw-r--r--  2.0 unx    46458 b- defN 24-Apr-24 00:28 determined/pytorch/_pytorch_context.py
--rw-r--r--  2.0 unx    69038 b- defN 24-Apr-24 00:28 determined/pytorch/_pytorch_trial.py
--rw-r--r--  2.0 unx    21628 b- defN 24-Apr-24 00:28 determined/pytorch/_reducer.py
--rw-r--r--  2.0 unx    14440 b- defN 24-Apr-24 00:28 determined/pytorch/_trainer.py
--rw-r--r--  2.0 unx     9561 b- defN 24-Apr-24 00:28 determined/pytorch/samplers.py
--rw-r--r--  2.0 unx      347 b- defN 24-Apr-24 00:28 determined/pytorch/deepspeed/__init__.py
--rw-r--r--  2.0 unx    19910 b- defN 24-Apr-24 00:28 determined/pytorch/deepspeed/_deepspeed_context.py
--rw-r--r--  2.0 unx    43011 b- defN 24-Apr-24 00:28 determined/pytorch/deepspeed/_deepspeed_trial.py
--rw-r--r--  2.0 unx     1984 b- defN 24-Apr-24 00:28 determined/pytorch/deepspeed/_mpu.py
--rw-r--r--  2.0 unx      771 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/__init__.py
--rw-r--r--  2.0 unx     1829 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/__main__.py
--rw-r--r--  2.0 unx    60130 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/_dsat_search_method.py
--rw-r--r--  2.0 unx     3601 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/_run_dsat.py
--rw-r--r--  2.0 unx    20180 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/_utils.py
--rw-r--r--  2.0 unx     2541 b- defN 24-Apr-24 00:28 determined/pytorch/dsat/defaults.py
--rw-r--r--  2.0 unx      175 b- defN 24-Apr-24 00:28 determined/pytorch/experimental/__init__.py
--rw-r--r--  2.0 unx    21611 b- defN 24-Apr-24 00:28 determined/pytorch/experimental/_torch_batch_process.py
--rw-r--r--  2.0 unx      343 b- defN 24-Apr-24 00:28 determined/searcher/__init__.py
--rw-r--r--  2.0 unx     4132 b- defN 24-Apr-24 00:28 determined/searcher/_remote_search_runner.py
--rw-r--r--  2.0 unx    16424 b- defN 24-Apr-24 00:28 determined/searcher/_search_method.py
--rw-r--r--  2.0 unx    15983 b- defN 24-Apr-24 00:28 determined/searcher/_search_runner.py
--rw-r--r--  2.0 unx      512 b- defN 24-Apr-24 00:28 determined/tensorboard/__init__.py
--rw-r--r--  2.0 unx     1579 b- defN 24-Apr-24 00:28 determined/tensorboard/azure.py
--rw-r--r--  2.0 unx     6108 b- defN 24-Apr-24 00:28 determined/tensorboard/base.py
--rw-r--r--  2.0 unx     4649 b- defN 24-Apr-24 00:28 determined/tensorboard/build.py
--rw-r--r--  2.0 unx      225 b- defN 24-Apr-24 00:28 determined/tensorboard/directory.py
--rw-r--r--  2.0 unx     2390 b- defN 24-Apr-24 00:28 determined/tensorboard/gcs.py
--rw-r--r--  2.0 unx     1883 b- defN 24-Apr-24 00:28 determined/tensorboard/s3.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-24 00:28 determined/tensorboard/shared.py
--rw-r--r--  2.0 unx     3787 b- defN 24-Apr-24 00:28 determined/tensorboard/util.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/__init__.py
--rw-r--r--  2.0 unx     2588 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/azure.py
--rw-r--r--  2.0 unx     1670 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/base.py
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/directory.py
--rw-r--r--  2.0 unx     1777 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/gcs.py
--rw-r--r--  2.0 unx     2521 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/s3.py
--rw-r--r--  2.0 unx     1685 b- defN 24-Apr-24 00:28 determined/tensorboard/fetchers/shared.py
--rw-r--r--  2.0 unx       91 b- defN 24-Apr-24 00:28 determined/tensorboard/metric_writers/__init__.py
--rw-r--r--  2.0 unx     3313 b- defN 24-Apr-24 00:28 determined/tensorboard/metric_writers/callback.py
--rw-r--r--  2.0 unx     3302 b- defN 24-Apr-24 00:28 determined/tensorboard/metric_writers/pytorch.py
--rw-r--r--  2.0 unx     4445 b- defN 24-Apr-24 00:28 determined/tensorboard/metric_writers/tensorflow.py
--rw-r--r--  2.0 unx       70 b- defN 24-Apr-24 00:28 determined/transformers/__init__.py
--rw-r--r--  2.0 unx    12928 b- defN 24-Apr-24 00:28 determined/transformers/_hf_callback.py
--rw-r--r--  2.0 unx     6068 b- defN 24-Apr-24 00:28 determined-0.31.1rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 00:28 determined-0.31.1rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-24 00:28 determined-0.31.1rc0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-24 00:28 determined-0.31.1rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    25154 b- defN 24-Apr-24 00:28 determined-0.31.1rc0.dist-info/RECORD
-273 files, 2926077 bytes uncompressed, 649169 bytes compressed:  77.8%
+Zip file size: 689295 bytes, number of entries: 273
+-rw-r--r--  2.0 unx     1140 b- defN 24-Apr-24 12:47 determined/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-24 12:47 determined/__version__.py
+-rw-r--r--  2.0 unx     1664 b- defN 24-Apr-24 12:47 determined/_env_context.py
+-rw-r--r--  2.0 unx     8854 b- defN 24-Apr-24 12:47 determined/_execution.py
+-rw-r--r--  2.0 unx     2779 b- defN 24-Apr-24 12:47 determined/_experiment_config.py
+-rw-r--r--  2.0 unx     4781 b- defN 24-Apr-24 12:47 determined/_import.py
+-rw-r--r--  2.0 unx    14970 b- defN 24-Apr-24 12:47 determined/_info.py
+-rw-r--r--  2.0 unx     1220 b- defN 24-Apr-24 12:47 determined/_trial.py
+-rw-r--r--  2.0 unx     4777 b- defN 24-Apr-24 12:47 determined/_trial_context.py
+-rw-r--r--  2.0 unx     3246 b- defN 24-Apr-24 12:47 determined/_trial_controller.py
+-rw-r--r--  2.0 unx     2271 b- defN 24-Apr-24 12:47 determined/constants.py
+-rw-r--r--  2.0 unx     2734 b- defN 24-Apr-24 12:47 determined/errors.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-Apr-24 12:47 determined/gpu.py
+-rw-r--r--  2.0 unx     6182 b- defN 24-Apr-24 12:47 determined/horovod.py
+-rw-r--r--  2.0 unx    20027 b- defN 24-Apr-24 12:47 determined/ipc.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-24 12:47 determined/load.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/py.typed
+-rw-r--r--  2.0 unx    18236 b- defN 24-Apr-24 12:47 determined/util.py
+-rw-r--r--  2.0 unx     6570 b- defN 24-Apr-24 12:47 determined/workload.py
+-rw-r--r--  2.0 unx      805 b- defN 24-Apr-24 12:47 determined/cli/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 24-Apr-24 12:47 determined/cli/__main__.py
+-rw-r--r--  2.0 unx     8425 b- defN 24-Apr-24 12:47 determined/cli/_declarative_argparse.py
+-rw-r--r--  2.0 unx     3968 b- defN 24-Apr-24 12:47 determined/cli/_util.py
+-rw-r--r--  2.0 unx    10013 b- defN 24-Apr-24 12:47 determined/cli/agent.py
+-rw-r--r--  2.0 unx     8306 b- defN 24-Apr-24 12:47 determined/cli/checkpoint.py
+-rw-r--r--  2.0 unx    10483 b- defN 24-Apr-24 12:47 determined/cli/cli.py
+-rw-r--r--  2.0 unx     5252 b- defN 24-Apr-24 12:47 determined/cli/command.py
+-rw-r--r--  2.0 unx    11680 b- defN 24-Apr-24 12:47 determined/cli/dev.py
+-rw-r--r--  2.0 unx      627 b- defN 24-Apr-24 12:47 determined/cli/errors.py
+-rw-r--r--  2.0 unx    52218 b- defN 24-Apr-24 12:47 determined/cli/experiment.py
+-rw-r--r--  2.0 unx     8714 b- defN 24-Apr-24 12:47 determined/cli/job.py
+-rw-r--r--  2.0 unx     4595 b- defN 24-Apr-24 12:47 determined/cli/master.py
+-rw-r--r--  2.0 unx     8479 b- defN 24-Apr-24 12:47 determined/cli/model.py
+-rw-r--r--  2.0 unx     7104 b- defN 24-Apr-24 12:47 determined/cli/notebook.py
+-rw-r--r--  2.0 unx    16661 b- defN 24-Apr-24 12:47 determined/cli/ntsc.py
+-rw-r--r--  2.0 unx     1870 b- defN 24-Apr-24 12:47 determined/cli/oauth.py
+-rw-r--r--  2.0 unx    11874 b- defN 24-Apr-24 12:47 determined/cli/project.py
+-rw-r--r--  2.0 unx     7918 b- defN 24-Apr-24 12:47 determined/cli/proxy.py
+-rw-r--r--  2.0 unx    18598 b- defN 24-Apr-24 12:47 determined/cli/rbac.py
+-rw-r--r--  2.0 unx    10204 b- defN 24-Apr-24 12:47 determined/cli/render.py
+-rw-r--r--  2.0 unx     5199 b- defN 24-Apr-24 12:47 determined/cli/resource_pool.py
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-24 12:47 determined/cli/resources.py
+-rw-r--r--  2.0 unx    13213 b- defN 24-Apr-24 12:47 determined/cli/shell.py
+-rw-r--r--  2.0 unx     5136 b- defN 24-Apr-24 12:47 determined/cli/sso.py
+-rw-r--r--  2.0 unx    13307 b- defN 24-Apr-24 12:47 determined/cli/task.py
+-rw-r--r--  2.0 unx     5300 b- defN 24-Apr-24 12:47 determined/cli/template.py
+-rw-r--r--  2.0 unx     7638 b- defN 24-Apr-24 12:47 determined/cli/tensorboard.py
+-rw-r--r--  2.0 unx      111 b- defN 24-Apr-24 12:47 determined/cli/top_arg_descriptions.py
+-rw-r--r--  2.0 unx    19091 b- defN 24-Apr-24 12:47 determined/cli/trial.py
+-rw-r--r--  2.0 unx     1635 b- defN 24-Apr-24 12:47 determined/cli/tunnel.py
+-rw-r--r--  2.0 unx    11091 b- defN 24-Apr-24 12:47 determined/cli/user.py
+-rw-r--r--  2.0 unx     8373 b- defN 24-Apr-24 12:47 determined/cli/user_groups.py
+-rw-r--r--  2.0 unx     2526 b- defN 24-Apr-24 12:47 determined/cli/version.py
+-rw-r--r--  2.0 unx    15325 b- defN 24-Apr-24 12:47 determined/cli/workspace.py
+-rw-r--r--  2.0 unx      352 b- defN 24-Apr-24 12:47 determined/common/__init__.py
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-24 12:47 determined/common/_logging.py
+-rw-r--r--  2.0 unx     8593 b- defN 24-Apr-24 12:47 determined/common/check.py
+-rw-r--r--  2.0 unx     2154 b- defN 24-Apr-24 12:47 determined/common/constants.py
+-rw-r--r--  2.0 unx     4278 b- defN 24-Apr-24 12:47 determined/common/context.py
+-rw-r--r--  2.0 unx     3569 b- defN 24-Apr-24 12:47 determined/common/detignore.py
+-rw-r--r--  2.0 unx     3328 b- defN 24-Apr-24 12:47 determined/common/detlomond.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/common/py.typed
+-rw-r--r--  2.0 unx     1662 b- defN 24-Apr-24 12:47 determined/common/requests.py
+-rw-r--r--  2.0 unx    11922 b- defN 24-Apr-24 12:47 determined/common/util.py
+-rw-r--r--  2.0 unx     1516 b- defN 24-Apr-24 12:47 determined/common/v1file_utils.py
+-rw-r--r--  2.0 unx      809 b- defN 24-Apr-24 12:47 determined/common/api/__init__.py
+-rw-r--r--  2.0 unx     4219 b- defN 24-Apr-24 12:47 determined/common/api/_rbac.py
+-rw-r--r--  2.0 unx     8891 b- defN 24-Apr-24 12:47 determined/common/api/_session.py
+-rw-r--r--  2.0 unx     6288 b- defN 24-Apr-24 12:47 determined/common/api/_util.py
+-rw-r--r--  2.0 unx     1469 b- defN 24-Apr-24 12:47 determined/common/api/analytics.py
+-rw-r--r--  2.0 unx    23171 b- defN 24-Apr-24 12:47 determined/common/api/authentication.py
+-rw-r--r--  2.0 unx   828044 b- defN 24-Apr-24 12:47 determined/common/api/bindings.py
+-rw-r--r--  2.0 unx     7421 b- defN 24-Apr-24 12:47 determined/common/api/certs.py
+-rw-r--r--  2.0 unx     4010 b- defN 24-Apr-24 12:47 determined/common/api/errors.py
+-rw-r--r--  2.0 unx     3281 b- defN 24-Apr-24 12:47 determined/common/api/logs.py
+-rw-r--r--  2.0 unx      247 b- defN 24-Apr-24 12:47 determined/common/api/metric.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-24 12:47 determined/common/experimental/__init__.py
+-rw-r--r--  2.0 unx      465 b- defN 24-Apr-24 12:47 determined/common/experimental/_util.py
+-rw-r--r--  2.0 unx    23950 b- defN 24-Apr-24 12:47 determined/common/experimental/determined.py
+-rw-r--r--  2.0 unx    26924 b- defN 24-Apr-24 12:47 determined/common/experimental/experiment.py
+-rw-r--r--  2.0 unx     3567 b- defN 24-Apr-24 12:47 determined/common/experimental/metrics.py
+-rw-r--r--  2.0 unx    16083 b- defN 24-Apr-24 12:47 determined/common/experimental/model.py
+-rw-r--r--  2.0 unx      306 b- defN 24-Apr-24 12:47 determined/common/experimental/oauth2_scim_client.py
+-rw-r--r--  2.0 unx     7712 b- defN 24-Apr-24 12:47 determined/common/experimental/project.py
+-rw-r--r--  2.0 unx     3607 b- defN 24-Apr-24 12:47 determined/common/experimental/resource_pool.py
+-rw-r--r--  2.0 unx    25650 b- defN 24-Apr-24 12:47 determined/common/experimental/trial.py
+-rw-r--r--  2.0 unx     5056 b- defN 24-Apr-24 12:47 determined/common/experimental/user.py
+-rw-r--r--  2.0 unx     5801 b- defN 24-Apr-24 12:47 determined/common/experimental/workspace.py
+-rw-r--r--  2.0 unx      170 b- defN 24-Apr-24 12:47 determined/common/experimental/checkpoint/__init__.py
+-rw-r--r--  2.0 unx    20350 b- defN 24-Apr-24 12:47 determined/common/experimental/checkpoint/_checkpoint.py
+-rw-r--r--  2.0 unx     4182 b- defN 24-Apr-24 12:47 determined/common/storage/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 24-Apr-24 12:47 determined/common/storage/_util.py
+-rw-r--r--  2.0 unx     4339 b- defN 24-Apr-24 12:47 determined/common/storage/azure.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-Apr-24 12:47 determined/common/storage/azure_client.py
+-rw-r--r--  2.0 unx     9368 b- defN 24-Apr-24 12:47 determined/common/storage/base.py
+-rw-r--r--  2.0 unx     4445 b- defN 24-Apr-24 12:47 determined/common/storage/boto3_credential_manager.py
+-rw-r--r--  2.0 unx     1014 b- defN 24-Apr-24 12:47 determined/common/storage/cloud.py
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-24 12:47 determined/common/storage/directory.py
+-rw-r--r--  2.0 unx     6479 b- defN 24-Apr-24 12:47 determined/common/storage/gcs.py
+-rw-r--r--  2.0 unx     6269 b- defN 24-Apr-24 12:47 determined/common/storage/s3.py
+-rw-r--r--  2.0 unx     9868 b- defN 24-Apr-24 12:47 determined/common/storage/shared.py
+-rw-r--r--  2.0 unx      243 b- defN 24-Apr-24 12:47 determined/common/streams/__init__.py
+-rw-r--r--  2.0 unx    19565 b- defN 24-Apr-24 12:47 determined/common/streams/_client.py
+-rw-r--r--  2.0 unx      391 b- defN 24-Apr-24 12:47 determined/common/streams/_util.py
+-rw-r--r--  2.0 unx     5357 b- defN 24-Apr-24 12:47 determined/common/streams/wire.py
+-rw-r--r--  2.0 unx     1405 b- defN 24-Apr-24 12:47 determined/core/__init__.py
+-rw-r--r--  2.0 unx    30354 b- defN 24-Apr-24 12:47 determined/core/_checkpoint.py
+-rw-r--r--  2.0 unx    14337 b- defN 24-Apr-24 12:47 determined/core/_context.py
+-rw-r--r--  2.0 unx    16604 b- defN 24-Apr-24 12:47 determined/core/_distributed.py
+-rw-r--r--  2.0 unx     2884 b- defN 24-Apr-24 12:47 determined/core/_experimental.py
+-rw-r--r--  2.0 unx     4580 b- defN 24-Apr-24 12:47 determined/core/_heartbeat.py
+-rw-r--r--  2.0 unx     5515 b- defN 24-Apr-24 12:47 determined/core/_log_shipper.py
+-rw-r--r--  2.0 unx     6620 b- defN 24-Apr-24 12:47 determined/core/_metrics.py
+-rw-r--r--  2.0 unx    12734 b- defN 24-Apr-24 12:47 determined/core/_preempt.py
+-rw-r--r--  2.0 unx    14841 b- defN 24-Apr-24 12:47 determined/core/_profiler.py
+-rw-r--r--  2.0 unx    15041 b- defN 24-Apr-24 12:47 determined/core/_searcher.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-24 12:47 determined/core/_tensorboard_mode.py
+-rw-r--r--  2.0 unx    11806 b- defN 24-Apr-24 12:47 determined/core/_train.py
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-24 12:47 determined/deploy/__init__.py
+-rw-r--r--  2.0 unx      996 b- defN 24-Apr-24 12:47 determined/deploy/cli.py
+-rw-r--r--  2.0 unx      855 b- defN 24-Apr-24 12:47 determined/deploy/errors.py
+-rw-r--r--  2.0 unx     2109 b- defN 24-Apr-24 12:47 determined/deploy/healthcheck.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/aws/__init__.py
+-rw-r--r--  2.0 unx    19820 b- defN 24-Apr-24 12:47 determined/deploy/aws/aws.py
+-rw-r--r--  2.0 unx    29379 b- defN 24-Apr-24 12:47 determined/deploy/aws/cli.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-Apr-24 12:47 determined/deploy/aws/constants.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-24 12:47 determined/deploy/aws/gen_vcpu_mapping.py
+-rw-r--r--  2.0 unx     2288 b- defN 24-Apr-24 12:47 determined/deploy/aws/master_config_inject.py
+-rw-r--r--  2.0 unx     5234 b- defN 24-Apr-24 12:47 determined/deploy/aws/preflight.py
+-rw-r--r--  2.0 unx    17324 b- defN 24-Apr-24 12:47 determined/deploy/aws/vcpu_mapping.yaml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/__init__.py
+-rw-r--r--  2.0 unx     6357 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/base.py
+-rw-r--r--  2.0 unx     1590 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/govcloud.py
+-rw-r--r--  2.0 unx     3131 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/secure.py
+-rw-r--r--  2.0 unx     1886 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/simple.py
+-rw-r--r--  2.0 unx     2381 b- defN 24-Apr-24 12:47 determined/deploy/aws/deployment_types/vpc.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/__init__.py
+-rw-r--r--  2.0 unx    30197 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/efs.yaml
+-rw-r--r--  2.0 unx    30907 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/fsx.yaml
+-rw-r--r--  2.0 unx    24534 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/govcloud.yaml
+-rw-r--r--  2.0 unx    32181 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/lore.yaml
+-rw-r--r--  2.0 unx    30070 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/secure.yaml
+-rw-r--r--  2.0 unx    26127 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/simple-rds.yaml
+-rw-r--r--  2.0 unx    25843 b- defN 24-Apr-24 12:47 determined/deploy/aws/templates/simple.yaml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/gcp/__init__.py
+-rw-r--r--  2.0 unx    25639 b- defN 24-Apr-24 12:47 determined/deploy/gcp/cli.py
+-rw-r--r--  2.0 unx      771 b- defN 24-Apr-24 12:47 determined/deploy/gcp/constants.py
+-rw-r--r--  2.0 unx    15054 b- defN 24-Apr-24 12:47 determined/deploy/gcp/gcp.py
+-rw-r--r--  2.0 unx     2494 b- defN 24-Apr-24 12:47 determined/deploy/gcp/preflight.py
+-rw-r--r--  2.0 unx     5428 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/main.tf
+-rw-r--r--  2.0 unx     1647 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/master.yaml.tmpl
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/outputs.tf
+-rw-r--r--  2.0 unx     3836 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/variables.tf
+-rw-r--r--  2.0 unx     6195 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/compute/main.tf
+-rw-r--r--  2.0 unx      424 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/compute/outputs.tf
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/compute/variables.tf
+-rw-r--r--  2.0 unx     1222 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/database/main.tf
+-rw-r--r--  2.0 unx      283 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/database/outputs.tf
+-rw-r--r--  2.0 unx      320 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/database/variables.tf
+-rw-r--r--  2.0 unx      522 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/filestore/main.tf
+-rw-r--r--  2.0 unx      184 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
+-rw-r--r--  2.0 unx      125 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/filestore/variables.tf
+-rw-r--r--  2.0 unx     1026 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/firewall/main.tf
+-rw-r--r--  2.0 unx      195 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
+-rw-r--r--  2.0 unx       75 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/firewall/variables.tf
+-rw-r--r--  2.0 unx      637 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/gcs/main.tf
+-rw-r--r--  2.0 unx       51 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/gcs/variables.tf
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/ip/main.tf
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/ip/outputs.tf
+-rw-r--r--  2.0 unx       88 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/ip/variables.tf
+-rw-r--r--  2.0 unx     1112 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/network/main.tf
+-rw-r--r--  2.0 unx      275 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/network/outputs.tf
+-rw-r--r--  2.0 unx      207 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/network/variables.tf
+-rw-r--r--  2.0 unx      962 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/service_account/main.tf
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-24 12:47 determined/deploy/gcp/terraform/modules/service_account/variables.tf
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/gke/__init__.py
+-rw-r--r--  2.0 unx    19788 b- defN 24-Apr-24 12:47 determined/deploy/gke/cli.py
+-rw-r--r--  2.0 unx      408 b- defN 24-Apr-24 12:47 determined/deploy/gke/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/deploy/local/__init__.py
+-rw-r--r--  2.0 unx    14111 b- defN 24-Apr-24 12:47 determined/deploy/local/cli.py
+-rw-r--r--  2.0 unx    17552 b- defN 24-Apr-24 12:47 determined/deploy/local/cluster_utils.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-24 12:47 determined/deploy/local/preflight.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/exec/__init__.py
+-rw-r--r--  2.0 unx     5473 b- defN 24-Apr-24 12:47 determined/exec/gc_checkpoints.py
+-rw-r--r--  2.0 unx     8475 b- defN 24-Apr-24 12:47 determined/exec/harness.py
+-rw-r--r--  2.0 unx     3695 b- defN 24-Apr-24 12:47 determined/exec/launch.py
+-rw-r--r--  2.0 unx      389 b- defN 24-Apr-24 12:47 determined/exec/pid_client.py
+-rw-r--r--  2.0 unx     1718 b- defN 24-Apr-24 12:47 determined/exec/pid_server.py
+-rw-r--r--  2.0 unx    13760 b- defN 24-Apr-24 12:47 determined/exec/prep_container.py
+-rw-r--r--  2.0 unx    11234 b- defN 24-Apr-24 12:47 determined/exec/tensorboard.py
+-rw-r--r--  2.0 unx      611 b- defN 24-Apr-24 12:47 determined/experimental/__init__.py
+-rw-r--r--  2.0 unx     3536 b- defN 24-Apr-24 12:47 determined/experimental/_native.py
+-rw-r--r--  2.0 unx    23124 b- defN 24-Apr-24 12:47 determined/experimental/client.py
+-rw-r--r--  2.0 unx      959 b- defN 24-Apr-24 12:47 determined/experimental/core_v2/__init__.py
+-rw-r--r--  2.0 unx     6430 b- defN 24-Apr-24 12:47 determined/experimental/core_v2/_core_context_v2.py
+-rw-r--r--  2.0 unx     8851 b- defN 24-Apr-24 12:47 determined/experimental/core_v2/_core_v2.py
+-rw-r--r--  2.0 unx     9851 b- defN 24-Apr-24 12:47 determined/experimental/core_v2/_unmanaged.py
+-rw-r--r--  2.0 unx      810 b- defN 24-Apr-24 12:47 determined/keras/__init__.py
+-rw-r--r--  2.0 unx     7579 b- defN 24-Apr-24 12:47 determined/keras/_data.py
+-rw-r--r--  2.0 unx    11491 b- defN 24-Apr-24 12:47 determined/keras/_enqueuer.py
+-rw-r--r--  2.0 unx     4342 b- defN 24-Apr-24 12:47 determined/keras/_load.py
+-rw-r--r--  2.0 unx      533 b- defN 24-Apr-24 12:47 determined/keras/_tensorboard_callback.py
+-rw-r--r--  2.0 unx    19133 b- defN 24-Apr-24 12:47 determined/keras/_tf_keras_context.py
+-rw-r--r--  2.0 unx     1251 b- defN 24-Apr-24 12:47 determined/keras/_tf_keras_multi_gpu.py
+-rw-r--r--  2.0 unx    48227 b- defN 24-Apr-24 12:47 determined/keras/_tf_keras_trial.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-24 12:47 determined/keras/_tf_rng.py
+-rw-r--r--  2.0 unx    27517 b- defN 24-Apr-24 12:47 determined/keras/callbacks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/launch/__init__.py
+-rw-r--r--  2.0 unx    15061 b- defN 24-Apr-24 12:47 determined/launch/deepspeed.py
+-rw-r--r--  2.0 unx    10762 b- defN 24-Apr-24 12:47 determined/launch/horovod.py
+-rw-r--r--  2.0 unx     4640 b- defN 24-Apr-24 12:47 determined/launch/torch_distributed.py
+-rw-r--r--  2.0 unx     6831 b- defN 24-Apr-24 12:47 determined/launch/wrap_rank.py
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 12:47 determined/layers/__init__.py
+-rw-r--r--  2.0 unx    19697 b- defN 24-Apr-24 12:47 determined/layers/_workload_sequencer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:47 determined/lightning/__init__.py
+-rw-r--r--  2.0 unx     1847 b- defN 24-Apr-24 12:47 determined/lightning/experimental.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-24 12:47 determined/pytorch/__init__.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-24 12:47 determined/pytorch/_callback.py
+-rw-r--r--  2.0 unx    16640 b- defN 24-Apr-24 12:47 determined/pytorch/_data.py
+-rw-r--r--  2.0 unx     3716 b- defN 24-Apr-24 12:47 determined/pytorch/_experimental.py
+-rw-r--r--  2.0 unx    12557 b- defN 24-Apr-24 12:47 determined/pytorch/_load.py
+-rw-r--r--  2.0 unx     3286 b- defN 24-Apr-24 12:47 determined/pytorch/_lr_scheduler.py
+-rw-r--r--  2.0 unx     8322 b- defN 24-Apr-24 12:47 determined/pytorch/_metric_utils.py
+-rw-r--r--  2.0 unx    46458 b- defN 24-Apr-24 12:47 determined/pytorch/_pytorch_context.py
+-rw-r--r--  2.0 unx    69038 b- defN 24-Apr-24 12:47 determined/pytorch/_pytorch_trial.py
+-rw-r--r--  2.0 unx    21628 b- defN 24-Apr-24 12:47 determined/pytorch/_reducer.py
+-rw-r--r--  2.0 unx    14440 b- defN 24-Apr-24 12:47 determined/pytorch/_trainer.py
+-rw-r--r--  2.0 unx     9561 b- defN 24-Apr-24 12:47 determined/pytorch/samplers.py
+-rw-r--r--  2.0 unx      347 b- defN 24-Apr-24 12:47 determined/pytorch/deepspeed/__init__.py
+-rw-r--r--  2.0 unx    19910 b- defN 24-Apr-24 12:47 determined/pytorch/deepspeed/_deepspeed_context.py
+-rw-r--r--  2.0 unx    43011 b- defN 24-Apr-24 12:47 determined/pytorch/deepspeed/_deepspeed_trial.py
+-rw-r--r--  2.0 unx     1984 b- defN 24-Apr-24 12:47 determined/pytorch/deepspeed/_mpu.py
+-rw-r--r--  2.0 unx      771 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/__init__.py
+-rw-r--r--  2.0 unx     1829 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/__main__.py
+-rw-r--r--  2.0 unx    60130 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/_dsat_search_method.py
+-rw-r--r--  2.0 unx     3601 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/_run_dsat.py
+-rw-r--r--  2.0 unx    20180 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/_utils.py
+-rw-r--r--  2.0 unx     2541 b- defN 24-Apr-24 12:47 determined/pytorch/dsat/defaults.py
+-rw-r--r--  2.0 unx      175 b- defN 24-Apr-24 12:47 determined/pytorch/experimental/__init__.py
+-rw-r--r--  2.0 unx    21611 b- defN 24-Apr-24 12:47 determined/pytorch/experimental/_torch_batch_process.py
+-rw-r--r--  2.0 unx      343 b- defN 24-Apr-24 12:47 determined/searcher/__init__.py
+-rw-r--r--  2.0 unx     4132 b- defN 24-Apr-24 12:47 determined/searcher/_remote_search_runner.py
+-rw-r--r--  2.0 unx    16424 b- defN 24-Apr-24 12:47 determined/searcher/_search_method.py
+-rw-r--r--  2.0 unx    15983 b- defN 24-Apr-24 12:47 determined/searcher/_search_runner.py
+-rw-r--r--  2.0 unx      512 b- defN 24-Apr-24 12:47 determined/tensorboard/__init__.py
+-rw-r--r--  2.0 unx     1579 b- defN 24-Apr-24 12:47 determined/tensorboard/azure.py
+-rw-r--r--  2.0 unx     6108 b- defN 24-Apr-24 12:47 determined/tensorboard/base.py
+-rw-r--r--  2.0 unx     4649 b- defN 24-Apr-24 12:47 determined/tensorboard/build.py
+-rw-r--r--  2.0 unx      225 b- defN 24-Apr-24 12:47 determined/tensorboard/directory.py
+-rw-r--r--  2.0 unx     2390 b- defN 24-Apr-24 12:47 determined/tensorboard/gcs.py
+-rw-r--r--  2.0 unx     1883 b- defN 24-Apr-24 12:47 determined/tensorboard/s3.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-24 12:47 determined/tensorboard/shared.py
+-rw-r--r--  2.0 unx     3787 b- defN 24-Apr-24 12:47 determined/tensorboard/util.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/__init__.py
+-rw-r--r--  2.0 unx     2588 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/azure.py
+-rw-r--r--  2.0 unx     1670 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/base.py
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/directory.py
+-rw-r--r--  2.0 unx     1777 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/gcs.py
+-rw-r--r--  2.0 unx     2521 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/s3.py
+-rw-r--r--  2.0 unx     1685 b- defN 24-Apr-24 12:47 determined/tensorboard/fetchers/shared.py
+-rw-r--r--  2.0 unx       91 b- defN 24-Apr-24 12:47 determined/tensorboard/metric_writers/__init__.py
+-rw-r--r--  2.0 unx     3313 b- defN 24-Apr-24 12:47 determined/tensorboard/metric_writers/callback.py
+-rw-r--r--  2.0 unx     3302 b- defN 24-Apr-24 12:47 determined/tensorboard/metric_writers/pytorch.py
+-rw-r--r--  2.0 unx     4445 b- defN 24-Apr-24 12:47 determined/tensorboard/metric_writers/tensorflow.py
+-rw-r--r--  2.0 unx       70 b- defN 24-Apr-24 12:47 determined/transformers/__init__.py
+-rw-r--r--  2.0 unx    12928 b- defN 24-Apr-24 12:47 determined/transformers/_hf_callback.py
+-rw-r--r--  2.0 unx     6068 b- defN 24-Apr-24 12:48 determined-0.32.0rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 12:48 determined-0.32.0rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-24 12:48 determined-0.32.0rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-24 12:48 determined-0.32.0rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    25154 b- defN 24-Apr-24 12:48 determined-0.32.0rc0.dist-info/RECORD
+273 files, 2926077 bytes uncompressed, 649167 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -798,23 +798,23 @@
 
 Filename: determined/transformers/__init__.py
 Comment: 
 
 Filename: determined/transformers/_hf_callback.py
 Comment: 
 
-Filename: determined-0.31.1rc0.dist-info/METADATA
+Filename: determined-0.32.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: determined-0.31.1rc0.dist-info/WHEEL
+Filename: determined-0.32.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: determined-0.31.1rc0.dist-info/entry_points.txt
+Filename: determined-0.32.0rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: determined-0.31.1rc0.dist-info/top_level.txt
+Filename: determined-0.32.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: determined-0.31.1rc0.dist-info/RECORD
+Filename: determined-0.32.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.31.1-rc0"
+__version__ = "0.32.0-rc0"
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
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
-    Default: 0.31.1-rc0
+    Default: 0.32.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   MaxAuxContainersPerAgent:
```

## Comparing `determined-0.31.1rc0.dist-info/METADATA` & `determined-0.32.0rc0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: determined
-Version: 0.31.1rc0
+Version: 0.32.0rc0
 Summary: Determined AI: The fastest and easiest way to build deep learning models.
 Home-page: https://determined.ai/
 Author: Determined AI
 Author-email: ai-open-source@hpe.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
```

## Comparing `determined-0.31.1rc0.dist-info/RECORD` & `determined-0.32.0rc0.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 determined/__init__.py,sha256=AylNLk96_lQOsbYJsIZYy-p9ElH-1qhuwRWvkNXqAtc,1140
-determined/__version__.py,sha256=CVred8ILq06uCytIgWbFVco-F3WepmbyLvGwBnGDHV0,27
+determined/__version__.py,sha256=9ozkgUU1AXNsj8bs51STfxrrnlYP8jHYOmLSQN-5gGo,27
 determined/_env_context.py,sha256=vG1rREr-gp-rVjGUn_5mzKhRxC8qv0RwpNY4rABT_h4,1664
 determined/_execution.py,sha256=FciLz0KifU2uxiZTOgDmuTTPyQj_mKeX90qNiU0IMS8,8854
 determined/_experiment_config.py,sha256=kkHvFHQzkI3HlckUozKwjfaieWIgeEot9jyPtvQuLjs,2779
 determined/_import.py,sha256=czaz1MQU8w2tfkeD3rIAVDpRyS_7lH0K9Sn-_zm2luQ,4781
 determined/_info.py,sha256=tc3R_0hwIRGRU7gx-lj4tLVbjjKJiZuQFGDkWBEwKCI,14970
 determined/_trial.py,sha256=7OagQh74mwD2FY6VHWTsKH6kiZIBrF_318gqRtcbtvc,1220
 determined/_trial_context.py,sha256=Ixhm5Tfj0emlOlTGkt57_WCqgO9njbchqM05ztldxkI,4777
@@ -131,21 +131,21 @@
 determined/deploy/aws/deployment_types/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/aws/deployment_types/base.py,sha256=LM39A0UMKJk6XhD59OAzQ_2vAoQN6f6Zs2HKyZ_mCQQ,6357
 determined/deploy/aws/deployment_types/govcloud.py,sha256=T09NNgMnXO66iJd2Xo2cQF222O_d18QGDj1P9hzCkWA,1590
 determined/deploy/aws/deployment_types/secure.py,sha256=sKtRW-wsgWAHveEt4I7fxbtlInKT1XV0-UOLhCCCKH4,3131
 determined/deploy/aws/deployment_types/simple.py,sha256=YJF8j4ALnwTSkE531MlxFC1ZZLlAVEsfsIescV_XJ4k,1886
 determined/deploy/aws/deployment_types/vpc.py,sha256=zU0ouLlRXs4kHrCPSQO85xnV4Y7wCKT9anjNNmnGW2M,2381
 determined/deploy/aws/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-determined/deploy/aws/templates/efs.yaml,sha256=yHsZfwJ43eutLYs-pY4leR2xqGrway9BhDNCGB-9W2I,30197
-determined/deploy/aws/templates/fsx.yaml,sha256=pj__dyQ7OnlYH0zgDonSWizt6DjWdpfy7pPOWpT7UKU,30907
-determined/deploy/aws/templates/govcloud.yaml,sha256=YueoUf5VhvZpZFB_TQTIr4VMUYb3RCKboBMrMXSL0X8,24534
-determined/deploy/aws/templates/lore.yaml,sha256=z3mTYthuxOZy0lbhyA_e3PvCxDv_mnnd5EOq_LwfQTw,32181
-determined/deploy/aws/templates/secure.yaml,sha256=bWXVDtjhBRgpUH2Zd2Hu_Ms3ujqs8Ekyy16xuRmvDDc,30070
-determined/deploy/aws/templates/simple-rds.yaml,sha256=060NScYSIyylWACNboPYCioH9J4r7UmYV0s-uwV5Ssc,26127
-determined/deploy/aws/templates/simple.yaml,sha256=ROeKOtGi_BL_08d1BfzNMZXZXlLUNB-YmncKETAWtjw,25843
+determined/deploy/aws/templates/efs.yaml,sha256=v080WIufOaH9973Rob1jcAOXlbHOccYq0vkZY9OP-2s,30197
+determined/deploy/aws/templates/fsx.yaml,sha256=k7ei1YS8JVHBkysyK2hp5Eh5H4ggmmHyrIsL6iC2y94,30907
+determined/deploy/aws/templates/govcloud.yaml,sha256=9do-8Ejx4nOFh4U8mjyQScyHKrghMJtisXubM8HLbCo,24534
+determined/deploy/aws/templates/lore.yaml,sha256=jczIPz9vdD3hTNZ06PQVEjDQOx6euBi2ggCDctNr-44,32181
+determined/deploy/aws/templates/secure.yaml,sha256=AWCxgdu8GdgUNUCW8Lw5tten3iMLYEdOQJncQ0o9Tdk,30070
+determined/deploy/aws/templates/simple-rds.yaml,sha256=cNd3qd1SzyrXlJi8SNPORYvVcCJB3bR09G27OajnTWI,26127
+determined/deploy/aws/templates/simple.yaml,sha256=LzMdjFSp9ffE00sLxdipYFMCJe_-4JYFHCePpVnfdOI,25843
 determined/deploy/gcp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/gcp/cli.py,sha256=lPCZDIEvLcHIAH3M755mgzXxwMIAKiDhzzIl_RVqGEE,25639
 determined/deploy/gcp/constants.py,sha256=M8J33nongOq5xBHi0ewwXsuuAWTfE72RW3ghGya9cyY,771
 determined/deploy/gcp/gcp.py,sha256=9WV8XPPfV7GW39-6BTqcw7k3e3u0azZuVK_cYAsDNtA,15054
 determined/deploy/gcp/preflight.py,sha256=no4VZjmb6MiAWCJZtKa2u9x2Efuv7fB8tg6u5-Qo6nE,2494
 determined/deploy/gcp/terraform/main.tf,sha256=x7gr1uL09albo6w0hFIe-09XC49rpz5UqiTDmQn2Qo4,5428
 determined/deploy/gcp/terraform/master.yaml.tmpl,sha256=D29nT4FTVAakjqaa_Ca8b2jim4LE_9EYOH00Ji4yvbE,1647
@@ -262,12 +262,12 @@
 determined/tensorboard/fetchers/shared.py,sha256=vEelW9B6Bf2e__1GTIBrxqWz9wJoDCFLLsBVUersUME,1685
 determined/tensorboard/metric_writers/__init__.py,sha256=QBZlDYJslTPnllbOOwzbV_XtKlsLwf9SR8YcL3MdJtY,91
 determined/tensorboard/metric_writers/callback.py,sha256=tmw-nFAe6uAhnEBL29LyjTf4chzOfhg2RIo2ANYm4Rw,3313
 determined/tensorboard/metric_writers/pytorch.py,sha256=2bH2ksaZUSYO-Xh9EKX64JGaSLijVRKC0pKrG9EK3Aw,3302
 determined/tensorboard/metric_writers/tensorflow.py,sha256=9YjN-BfWfsoP9o83iHbrIi6BGcLTKjahv6du-swBoyY,4445
 determined/transformers/__init__.py,sha256=WJSvfLUkyIXjrbAKEe-SRXYdl8ZuDceqztiZ0ASJKIA,70
 determined/transformers/_hf_callback.py,sha256=ZkHyttQK9Uy9dCts-TbNqyjcpL0d4egkd_hbKTjBWLY,12928
-determined-0.31.1rc0.dist-info/METADATA,sha256=5rXy3OLVh899GL4FTisUMZKczBH91IGu2wUevKhZo8s,6068
-determined-0.31.1rc0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-determined-0.31.1rc0.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
-determined-0.31.1rc0.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
-determined-0.31.1rc0.dist-info/RECORD,,
+determined-0.32.0rc0.dist-info/METADATA,sha256=yo-26D28zjbieZpr_2QCHjEGSpGZD5W_hx5whq9ANv0,6068
+determined-0.32.0rc0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+determined-0.32.0rc0.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
+determined-0.32.0rc0.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
+determined-0.32.0rc0.dist-info/RECORD,,
```

