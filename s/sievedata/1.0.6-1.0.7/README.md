# Comparing `tmp/sievedata-1.0.6-py3-none-any.whl.zip` & `tmp/sievedata-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,183 +1,104 @@
-Zip file size: 231415 bytes, number of entries: 181
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 08:15 cli/__init__.py
--rw-r--r--  2.0 unx     7672 b- defN 24-Jan-11 00:32 cli/sieve.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 08:15 cli/commands/__init__.py
--rw-r--r--  2.0 unx     1106 b- defN 23-Aug-07 21:11 cli/commands/feedback.py
--rw-r--r--  2.0 unx     1130 b- defN 23-Oct-05 07:40 cli/commands/job.py
--rw-r--r--  2.0 unx     1161 b- defN 23-Oct-05 07:40 cli/commands/model.py
--rw-r--r--  2.0 unx     3136 b- defN 23-Aug-07 21:11 cli/commands/projects.py
--rw-r--r--  2.0 unx     1518 b- defN 23-Aug-07 21:11 cli/commands/query.py
--rw-r--r--  2.0 unx     1143 b- defN 23-Oct-05 07:40 cli/commands/secret.py
--rw-r--r--  2.0 unx     2712 b- defN 23-Aug-07 21:11 cli/commands/weights.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Oct-05 07:40 cli/commands/workflow.py
--rw-r--r--  2.0 unx      592 b- defN 24-Mar-26 02:04 sieve/__init__.py
--rw-r--r--  2.0 unx     2154 b- defN 23-Nov-21 00:45 sieve/serialization.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:04 sieve/_cli/__init__.py
--rw-r--r--  2.0 unx     6078 b- defN 24-Apr-19 01:39 sieve/_cli/sieve.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:04 sieve/_cli/commands/__init__.py
--rw-r--r--  2.0 unx     1284 b- defN 24-Mar-26 00:04 sieve/_cli/commands/job.py
--rw-r--r--  2.0 unx     1315 b- defN 24-Mar-26 00:04 sieve/_cli/commands/model.py
--rw-r--r--  2.0 unx     1734 b- defN 24-Mar-26 02:04 sieve/_cli/commands/secret.py
--rw-r--r--  2.0 unx     1270 b- defN 24-Mar-26 00:04 sieve/_cli/commands/workflow.py
--rw-r--r--  2.0 unx     2550 b- defN 24-Mar-26 02:04 sieve/_openapi/__init__.py
--rw-r--r--  2.0 unx    25793 b- defN 24-Mar-26 02:04 sieve/_openapi/api_client.py
--rw-r--r--  2.0 unx      652 b- defN 24-Mar-26 02:04 sieve/_openapi/api_response.py
--rw-r--r--  2.0 unx    15355 b- defN 24-Mar-26 02:04 sieve/_openapi/configuration.py
--rw-r--r--  2.0 unx     5974 b- defN 24-Mar-26 02:04 sieve/_openapi/exceptions.py
--rw-r--r--  2.0 unx     9234 b- defN 24-Mar-26 02:04 sieve/_openapi/rest.py
--rw-r--r--  2.0 unx      102 b- defN 24-Mar-26 02:04 sieve/_openapi/api/__init__.py
--rw-r--r--  2.0 unx   257843 b- defN 24-Mar-26 02:04 sieve/_openapi/api/default_api.py
--rw-r--r--  2.0 unx     1952 b- defN 24-Mar-26 02:04 sieve/_openapi/models/__init__.py
--rw-r--r--  2.0 unx     4870 b- defN 24-Mar-21 01:06 sieve/_openapi/models/active.py
--rw-r--r--  2.0 unx     4942 b- defN 24-Mar-21 01:06 sieve/_openapi/models/awaiting_resources.py
--rw-r--r--  2.0 unx     2878 b- defN 24-Mar-26 02:04 sieve/_openapi/models/body_get_upload_url_v1_upload_url_post.py
--rw-r--r--  2.0 unx     4927 b- defN 24-Mar-21 01:06 sieve/_openapi/models/built_at.py
--rw-r--r--  2.0 unx     4961 b- defN 24-Mar-21 01:06 sieve/_openapi/models/children.py
--rw-r--r--  2.0 unx     4839 b- defN 24-Mar-21 01:06 sieve/_openapi/models/code_url.py
--rw-r--r--  2.0 unx     4928 b- defN 24-Mar-21 01:06 sieve/_openapi/models/completed_at.py
--rw-r--r--  2.0 unx     5357 b- defN 24-Mar-26 02:04 sieve/_openapi/models/config_model.py
--rw-r--r--  2.0 unx     4870 b- defN 24-Mar-21 01:06 sieve/_openapi/models/cover_image_url.py
--rw-r--r--  2.0 unx     4916 b- defN 24-Mar-21 01:06 sieve/_openapi/models/created_at.py
--rw-r--r--  2.0 unx     4835 b- defN 24-Mar-21 01:06 sieve/_openapi/models/cuda_version.py
--rw-r--r--  2.0 unx     4820 b- defN 24-Mar-21 01:06 sieve/_openapi/models/data.py
--rw-r--r--  2.0 unx     4844 b- defN 24-Mar-21 01:06 sieve/_openapi/models/default.py
--rw-r--r--  2.0 unx     4867 b- defN 24-Mar-21 01:06 sieve/_openapi/models/description.py
--rw-r--r--  2.0 unx     4859 b- defN 24-Mar-21 01:06 sieve/_openapi/models/description1.py
--rw-r--r--  2.0 unx     4857 b- defN 24-Mar-21 01:06 sieve/_openapi/models/description2.py
--rw-r--r--  2.0 unx     4851 b- defN 24-Mar-21 01:06 sieve/_openapi/models/end_timestamp.py
--rw-r--r--  2.0 unx     4809 b- defN 24-Mar-21 01:06 sieve/_openapi/models/env.py
--rw-r--r--  2.0 unx     3187 b- defN 24-Mar-26 02:04 sieve/_openapi/models/environment_variable.py
--rw-r--r--  2.0 unx     4862 b- defN 24-Mar-21 01:06 sieve/_openapi/models/environment_variables.py
--rw-r--r--  2.0 unx     4859 b- defN 24-Mar-21 01:06 sieve/_openapi/models/error.py
--rw-r--r--  2.0 unx     4866 b- defN 24-Mar-21 01:06 sieve/_openapi/models/featured_key.py
--rw-r--r--  2.0 unx     5113 b- defN 24-Mar-26 02:04 sieve/_openapi/models/function.py
--rw-r--r--  2.0 unx     7034 b- defN 24-Mar-26 02:04 sieve/_openapi/models/function_app.py
--rw-r--r--  2.0 unx     4892 b- defN 24-Mar-21 01:06 sieve/_openapi/models/function_type.py
--rw-r--r--  2.0 unx     2972 b- defN 24-Mar-26 02:04 sieve/_openapi/models/http_validation_error.py
--rw-r--r--  2.0 unx     4783 b- defN 24-Mar-21 01:06 sieve/_openapi/models/id.py
--rw-r--r--  2.0 unx     2437 b- defN 24-Mar-26 02:04 sieve/_openapi/models/id_response.py
--rw-r--r--  2.0 unx     4887 b- defN 24-Mar-21 01:06 sieve/_openapi/models/idle.py
--rw-r--r--  2.0 unx     3930 b- defN 24-Mar-26 02:04 sieve/_openapi/models/input_output.py
--rw-r--r--  2.0 unx     4936 b- defN 24-Mar-30 00:44 sieve/_openapi/models/inputs.py
--rw-r--r--  2.0 unx     6414 b- defN 24-Mar-26 02:04 sieve/_openapi/models/job.py
--rw-r--r--  2.0 unx     4876 b- defN 24-Mar-21 01:06 sieve/_openapi/models/job_function.py
--rw-r--r--  2.0 unx     4976 b- defN 24-Mar-26 02:04 sieve/_openapi/models/job_outputs_inner.py
--rw-r--r--  2.0 unx     3002 b- defN 24-Mar-26 02:04 sieve/_openapi/models/list_function_jobs_response.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Mar-26 02:04 sieve/_openapi/models/list_response_job.py
--rw-r--r--  2.0 unx     2990 b- defN 24-Mar-26 02:04 sieve/_openapi/models/list_response_secret.py
--rw-r--r--  2.0 unx     4831 b- defN 24-Mar-26 02:04 sieve/_openapi/models/location_inner.py
--rw-r--r--  2.0 unx     4958 b- defN 24-Mar-21 01:06 sieve/_openapi/models/maximum_replicas.py
--rw-r--r--  2.0 unx     4803 b- defN 24-Mar-21 01:06 sieve/_openapi/models/model_schema.py
--rw-r--r--  2.0 unx     4810 b- defN 24-Mar-21 01:06 sieve/_openapi/models/name.py
--rw-r--r--  2.0 unx     2771 b- defN 24-Mar-26 02:04 sieve/_openapi/models/organization_model.py
--rw-r--r--  2.0 unx     4793 b- defN 24-Mar-21 01:06 sieve/_openapi/models/outputs.py
--rw-r--r--  2.0 unx     4974 b- defN 24-Mar-26 02:04 sieve/_openapi/models/push_request.py
--rw-r--r--  2.0 unx     3616 b- defN 24-Mar-26 02:04 sieve/_openapi/models/push_response.py
--rw-r--r--  2.0 unx     4924 b- defN 24-Mar-21 01:06 sieve/_openapi/models/queued_at.py
--rw-r--r--  2.0 unx     4824 b- defN 24-Mar-21 01:06 sieve/_openapi/models/readme.py
--rw-r--r--  2.0 unx     4925 b- defN 24-Mar-21 01:06 sieve/_openapi/models/ready_at.py
--rw-r--r--  2.0 unx     4815 b- defN 24-Mar-21 01:06 sieve/_openapi/models/run_id.py
--rw-r--r--  2.0 unx     2716 b- defN 24-Mar-26 02:04 sieve/_openapi/models/secret.py
--rw-r--r--  2.0 unx     4880 b- defN 24-Mar-21 01:06 sieve/_openapi/models/setup.py
--rw-r--r--  2.0 unx     4863 b- defN 24-Mar-21 01:06 sieve/_openapi/models/start_timestamp.py
--rw-r--r--  2.0 unx     4939 b- defN 24-Mar-21 01:06 sieve/_openapi/models/started_at.py
--rw-r--r--  2.0 unx     5039 b- defN 24-Mar-21 01:06 sieve/_openapi/models/starting.py
--rw-r--r--  2.0 unx     2528 b- defN 24-Mar-26 02:04 sieve/_openapi/models/status_response.py
--rw-r--r--  2.0 unx     4863 b- defN 24-Mar-21 01:06 sieve/_openapi/models/stream_output.py
--rw-r--r--  2.0 unx     4781 b- defN 24-Mar-21 01:06 sieve/_openapi/models/tags.py
--rw-r--r--  2.0 unx     4908 b- defN 24-Mar-21 01:06 sieve/_openapi/models/type.py
--rw-r--r--  2.0 unx     2818 b- defN 24-Mar-26 02:04 sieve/_openapi/models/upload_model.py
--rw-r--r--  2.0 unx     2667 b- defN 24-Mar-26 02:04 sieve/_openapi/models/upload_url_response.py
--rw-r--r--  2.0 unx     2741 b- defN 24-Mar-26 02:04 sieve/_openapi/models/user_model.py
--rw-r--r--  2.0 unx     3031 b- defN 24-Mar-26 02:04 sieve/_openapi/models/validation_error.py
--rw-r--r--  2.0 unx     4891 b- defN 24-Mar-21 01:06 sieve/_openapi/models/validation_error_loc_inner.py
--rw-r--r--  2.0 unx     8813 b- defN 24-Mar-26 02:04 sieve/_openapi/models/version.py
--rw-r--r--  2.0 unx     4944 b- defN 24-Mar-21 01:06 sieve/_openapi/models/version_current_workers.py
--rw-r--r--  2.0 unx     2804 b- defN 24-Mar-26 02:04 sieve/_openapi/models/webhook_model.py
--rw-r--r--  2.0 unx     4818 b- defN 24-Mar-21 01:06 sieve/_openapi/models/webhooks.py
--rw-r--r--  2.0 unx     4877 b- defN 24-Mar-21 01:06 sieve/_openapi/models/webhooks1.py
--rw-r--r--  2.0 unx     3977 b- defN 24-Mar-26 02:04 sieve/_openapi/models/worker_counts.py
--rw-r--r--  2.0 unx     4841 b- defN 24-Mar-21 01:06 sieve/_openapi/models/workflow_id.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 01:06 sieve/_openapi/test/__init__.py
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-20 04:48 sieve/api/__init__.py
--rw-r--r--  2.0 unx      319 b- defN 23-Aug-07 21:11 sieve/api/auth.py
--rw-r--r--  2.0 unx    22175 b- defN 23-Aug-07 21:11 sieve/api/client.py
--rw-r--r--  2.0 unx    16490 b- defN 24-Apr-20 01:05 sieve/api/common.py
--rw-r--r--  2.0 unx      618 b- defN 23-Oct-05 07:40 sieve/api/constants.py
--rw-r--r--  2.0 unx     6305 b- defN 24-Apr-20 01:05 sieve/api/utils.py
--rw-r--r--  2.0 unx       52 b- defN 24-Mar-26 00:04 sieve/api/jobs/__init__.py
--rw-r--r--  2.0 unx     1632 b- defN 24-Mar-26 00:04 sieve/api/jobs/common.py
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-26 02:04 sieve/api/models/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 24-Mar-26 02:04 sieve/api/models/common.py
--rw-r--r--  2.0 unx       54 b- defN 23-Aug-07 21:11 sieve/api/secrets/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 24-Mar-26 02:04 sieve/api/secrets/common.py
--rw-r--r--  2.0 unx       47 b- defN 24-Mar-26 00:04 sieve/api/workflows/__init__.py
--rw-r--r--  2.0 unx     1244 b- defN 24-Mar-26 00:04 sieve/api/workflows/common.py
--rw-r--r--  2.0 unx        1 b- defN 23-Jan-25 08:15 sieve/api_v12/__init__.py
--rw-r--r--  2.0 unx      296 b- defN 23-Jan-25 08:15 sieve/api_v12/auth.py
--rw-r--r--  2.0 unx    21927 b- defN 23-Jan-25 08:15 sieve/api_v12/client.py
--rw-r--r--  2.0 unx    12919 b- defN 23-Mar-09 01:11 sieve/api_v12/common.py
--rw-r--r--  2.0 unx      896 b- defN 23-Feb-20 23:42 sieve/api_v12/constants.py
--rw-r--r--  2.0 unx      376 b- defN 23-Jan-30 22:56 sieve/api_v12/utils.py
--rw-r--r--  2.0 unx       51 b- defN 23-Jan-25 08:15 sieve/api_v12/jobs/__init__.py
--rw-r--r--  2.0 unx     2048 b- defN 23-Feb-20 23:42 sieve/api_v12/jobs/common.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jan-25 08:15 sieve/api_v12/models/__init__.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jan-25 08:15 sieve/api_v12/models/common.py
--rw-r--r--  2.0 unx       53 b- defN 23-Mar-09 01:11 sieve/api_v12/secrets/__init__.py
--rw-r--r--  2.0 unx     1893 b- defN 23-Mar-09 01:11 sieve/api_v12/secrets/common.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jan-25 08:15 sieve/api_v12/workflows/__init__.py
--rw-r--r--  2.0 unx     1774 b- defN 23-Jan-30 22:56 sieve/api_v12/workflows/common.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 08:15 sieve/functions/__init__.py
--rw-r--r--  2.0 unx      866 b- defN 23-Jan-25 08:15 sieve/functions/common.py
--rw-r--r--  2.0 unx    31068 b- defN 24-Apr-20 00:32 sieve/functions/function.py
--rw-r--r--  2.0 unx     2008 b- defN 23-Jan-25 08:15 sieve/functions/helpers.py
--rw-r--r--  2.0 unx     9612 b- defN 24-Mar-26 00:04 sieve/functions/reference.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Mar-26 02:04 sieve/functions/utils.py
--rw-r--r--  2.0 unx       75 b- defN 23-Jan-25 08:15 sieve/predictors/__init__.py
--rw-r--r--  2.0 unx     1896 b- defN 23-Jan-25 08:15 sieve/predictors/predictors.py
--rw-r--r--  2.0 unx     1123 b- defN 23-Jan-25 08:15 sieve/predictors/trainable.py
--rw-r--r--  2.0 unx     5235 b- defN 23-Jan-25 08:15 sieve/predictors/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/env/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 23-Oct-05 07:40 sieve/server/env/env.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/grpc/__init__.py
--rw-r--r--  2.0 unx     9633 b- defN 23-Nov-21 19:20 sieve/server/grpc/runner.py
--rw-r--r--  2.0 unx     1895 b- defN 24-Mar-26 02:04 sieve/server/grpc/serializer.py
--rw-r--r--  2.0 unx     9310 b- defN 24-Apr-19 19:10 sieve/server/grpc/simple_grpc_server.py
--rw-r--r--  2.0 unx     6735 b- defN 24-Apr-19 19:10 sieve/server/grpc/worker.py
--rw-r--r--  2.0 unx       55 b- defN 23-Aug-07 21:11 sieve/server/grpc/constants/__init__.py
--rw-r--r--  2.0 unx       95 b- defN 23-Aug-07 21:11 sieve/server/grpc/constants/constants.py
--rw-r--r--  2.0 unx      258 b- defN 23-Aug-07 21:11 sieve/server/grpc/message/__init__.py
--rw-r--r--  2.0 unx      437 b- defN 23-Oct-05 07:40 sieve/server/grpc/message/error_response.py
--rw-r--r--  2.0 unx     5342 b- defN 24-Jan-11 00:32 sieve/server/grpc/message/iterator_input.py
--rw-r--r--  2.0 unx     7278 b- defN 24-Apr-18 21:23 sieve/server/grpc/message/iterator_output.py
--rw-r--r--  2.0 unx     2369 b- defN 24-Jan-11 00:32 sieve/server/grpc/message/single_input.py
--rw-r--r--  2.0 unx     1038 b- defN 24-Jan-11 00:32 sieve/server/grpc/message/single_output.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/handling/__init__.py
--rw-r--r--  2.0 unx    12669 b- defN 24-Mar-26 02:04 sieve/server/handling/file_handling.py
--rw-r--r--  2.0 unx     2186 b- defN 23-Oct-05 07:40 sieve/server/handling/sys_handling.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/logging/__init__.py
--rw-r--r--  2.0 unx     5296 b- defN 24-Apr-19 19:10 sieve/server/logging/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 04:48 sieve/server/proto/__init__.py
--rw-r--r--  2.0 unx     2588 b- defN 24-Mar-26 02:04 sieve/server/proto/server_pb2.py
--rw-r--r--  2.0 unx     2307 b- defN 24-Mar-26 02:04 sieve/server/proto/server_pb2.pyi
--rw-r--r--  2.0 unx     6063 b- defN 24-Mar-26 02:04 sieve/server/proto/server_pb2_grpc.py
--rw-r--r--  2.0 unx     3589 b- defN 24-Jan-11 00:32 sieve/server/proto/worker_pb2.py
--rw-r--r--  2.0 unx     3975 b- defN 24-Jan-11 00:32 sieve/server/proto/worker_pb2.pyi
--rw-r--r--  2.0 unx     6122 b- defN 23-Oct-05 07:40 sieve/server/proto/worker_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 08:15 sieve/types/__init__.py
--rw-r--r--  2.0 unx      635 b- defN 24-Mar-26 02:04 sieve/types/base.py
--rw-r--r--  2.0 unx      817 b- defN 23-Aug-07 21:11 sieve/types/box.py
--rw-r--r--  2.0 unx      176 b- defN 23-Aug-07 21:11 sieve/types/embedding.py
--rw-r--r--  2.0 unx    26598 b- defN 24-Mar-26 02:04 sieve/types/file.py
--rw-r--r--  2.0 unx      333 b- defN 24-Mar-26 02:04 sieve/types/metadata.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 00:04 sieve/workflows/__init__.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Mar-26 00:04 sieve/workflows/config.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Mar-26 00:04 sieve/workflows/workflow.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      943 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    15873 b- defN 24-Apr-22 17:47 sievedata-1.0.6.dist-info/RECORD
-181 files, 965688 bytes uncompressed, 206241 bytes compressed:  78.6%
+Zip file size: 131715 bytes, number of entries: 102
+-rw-r--r--  2.0 unx      592 b- defN 24-Mar-25 21:36 sieve/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/_cli/__init__.py
+-rw-r--r--  2.0 unx     6113 b- defN 24-Apr-23 17:56 sieve/_cli/sieve.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/_cli/commands/__init__.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-Mar-25 19:35 sieve/_cli/commands/job.py
+-rw-r--r--  2.0 unx     1315 b- defN 24-Mar-25 19:35 sieve/_cli/commands/model.py
+-rw-r--r--  2.0 unx     1734 b- defN 24-Mar-25 21:36 sieve/_cli/commands/secret.py
+-rw-r--r--  2.0 unx     1270 b- defN 24-Mar-25 19:35 sieve/_cli/commands/workflow.py
+-rw-r--r--  2.0 unx     2550 b- defN 24-Mar-25 21:48 sieve/_openapi/__init__.py
+-rw-r--r--  2.0 unx    25793 b- defN 24-Mar-25 21:48 sieve/_openapi/api_client.py
+-rw-r--r--  2.0 unx      652 b- defN 24-Mar-25 21:48 sieve/_openapi/api_response.py
+-rw-r--r--  2.0 unx    15355 b- defN 24-Mar-25 21:48 sieve/_openapi/configuration.py
+-rw-r--r--  2.0 unx     5974 b- defN 24-Mar-25 21:48 sieve/_openapi/exceptions.py
+-rw-r--r--  2.0 unx     9234 b- defN 24-Mar-25 21:48 sieve/_openapi/rest.py
+-rw-r--r--  2.0 unx      102 b- defN 24-Mar-25 21:48 sieve/_openapi/api/__init__.py
+-rw-r--r--  2.0 unx   257843 b- defN 24-Mar-25 21:48 sieve/_openapi/api/default_api.py
+-rw-r--r--  2.0 unx     1952 b- defN 24-Mar-25 21:48 sieve/_openapi/models/__init__.py
+-rw-r--r--  2.0 unx     2878 b- defN 24-Mar-25 21:48 sieve/_openapi/models/body_get_upload_url_v1_upload_url_post.py
+-rw-r--r--  2.0 unx     5357 b- defN 24-Mar-25 21:48 sieve/_openapi/models/config_model.py
+-rw-r--r--  2.0 unx     3187 b- defN 24-Mar-25 21:48 sieve/_openapi/models/environment_variable.py
+-rw-r--r--  2.0 unx     5113 b- defN 24-Mar-25 21:36 sieve/_openapi/models/function.py
+-rw-r--r--  2.0 unx     7034 b- defN 24-Mar-25 21:48 sieve/_openapi/models/function_app.py
+-rw-r--r--  2.0 unx     2972 b- defN 24-Mar-25 21:48 sieve/_openapi/models/http_validation_error.py
+-rw-r--r--  2.0 unx     2437 b- defN 24-Mar-25 21:48 sieve/_openapi/models/id_response.py
+-rw-r--r--  2.0 unx     3930 b- defN 24-Apr-12 22:32 sieve/_openapi/models/input_output.py
+-rw-r--r--  2.0 unx     4936 b- defN 24-Apr-12 22:32 sieve/_openapi/models/inputs.py
+-rw-r--r--  2.0 unx     6414 b- defN 24-Mar-25 21:48 sieve/_openapi/models/job.py
+-rw-r--r--  2.0 unx     4976 b- defN 24-Mar-25 21:48 sieve/_openapi/models/job_outputs_inner.py
+-rw-r--r--  2.0 unx     3002 b- defN 24-Mar-25 21:36 sieve/_openapi/models/list_function_jobs_response.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Mar-25 21:48 sieve/_openapi/models/list_response_job.py
+-rw-r--r--  2.0 unx     2990 b- defN 24-Mar-25 21:48 sieve/_openapi/models/list_response_secret.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-Mar-25 21:48 sieve/_openapi/models/location_inner.py
+-rw-r--r--  2.0 unx     2771 b- defN 24-Mar-25 21:48 sieve/_openapi/models/organization_model.py
+-rw-r--r--  2.0 unx     4974 b- defN 24-Mar-28 17:36 sieve/_openapi/models/push_request.py
+-rw-r--r--  2.0 unx     3616 b- defN 24-Mar-25 21:48 sieve/_openapi/models/push_response.py
+-rw-r--r--  2.0 unx     2716 b- defN 24-Mar-25 21:48 sieve/_openapi/models/secret.py
+-rw-r--r--  2.0 unx     2528 b- defN 24-Mar-25 21:48 sieve/_openapi/models/status_response.py
+-rw-r--r--  2.0 unx     2818 b- defN 24-Mar-25 21:48 sieve/_openapi/models/upload_model.py
+-rw-r--r--  2.0 unx     2667 b- defN 24-Mar-25 21:48 sieve/_openapi/models/upload_url_response.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-Mar-25 21:48 sieve/_openapi/models/user_model.py
+-rw-r--r--  2.0 unx     3031 b- defN 24-Mar-25 21:48 sieve/_openapi/models/validation_error.py
+-rw-r--r--  2.0 unx     8813 b- defN 24-Mar-25 21:48 sieve/_openapi/models/version.py
+-rw-r--r--  2.0 unx     2804 b- defN 24-Mar-25 21:48 sieve/_openapi/models/webhook_model.py
+-rw-r--r--  2.0 unx     3977 b- defN 24-Mar-25 21:48 sieve/_openapi/models/worker_counts.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 21:48 sieve/_openapi/test/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Feb-12 21:35 sieve/api/__init__.py
+-rw-r--r--  2.0 unx    16526 b- defN 24-Apr-23 17:56 sieve/api/common.py
+-rw-r--r--  2.0 unx      618 b- defN 24-Feb-12 21:35 sieve/api/constants.py
+-rw-r--r--  2.0 unx     6305 b- defN 24-Apr-19 16:19 sieve/api/utils.py
+-rw-r--r--  2.0 unx       52 b- defN 24-Mar-25 19:35 sieve/api/jobs/__init__.py
+-rw-r--r--  2.0 unx     1632 b- defN 24-Mar-25 19:36 sieve/api/jobs/common.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Mar-25 21:36 sieve/api/models/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 24-Mar-25 21:36 sieve/api/models/common.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Feb-12 21:35 sieve/api/secrets/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 24-Mar-25 21:36 sieve/api/secrets/common.py
+-rw-r--r--  2.0 unx       47 b- defN 24-Mar-25 19:35 sieve/api/workflows/__init__.py
+-rw-r--r--  2.0 unx     1244 b- defN 24-Mar-25 19:36 sieve/api/workflows/common.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/functions/__init__.py
+-rw-r--r--  2.0 unx    31068 b- defN 24-Apr-12 22:32 sieve/functions/function.py
+-rw-r--r--  2.0 unx     9612 b- defN 24-Mar-25 19:35 sieve/functions/reference.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Apr-23 17:43 sieve/functions/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/env/__init__.py
+-rw-r--r--  2.0 unx      510 b- defN 24-Feb-12 21:35 sieve/server/env/env.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/grpc/__init__.py
+-rw-r--r--  2.0 unx     9633 b- defN 24-Apr-18 21:06 sieve/server/grpc/runner.py
+-rw-r--r--  2.0 unx     1895 b- defN 24-Mar-25 19:36 sieve/server/grpc/serializer.py
+-rw-r--r--  2.0 unx     9310 b- defN 24-Apr-23 17:56 sieve/server/grpc/simple_grpc_server.py
+-rw-r--r--  2.0 unx     6735 b- defN 24-Apr-23 17:56 sieve/server/grpc/worker.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Feb-12 21:35 sieve/server/grpc/constants/__init__.py
+-rw-r--r--  2.0 unx       95 b- defN 24-Feb-12 21:35 sieve/server/grpc/constants/constants.py
+-rw-r--r--  2.0 unx      258 b- defN 24-Feb-12 21:35 sieve/server/grpc/message/__init__.py
+-rw-r--r--  2.0 unx      437 b- defN 24-Feb-12 21:35 sieve/server/grpc/message/error_response.py
+-rw-r--r--  2.0 unx     5342 b- defN 24-Feb-12 21:35 sieve/server/grpc/message/iterator_input.py
+-rw-r--r--  2.0 unx     7278 b- defN 24-Feb-12 21:35 sieve/server/grpc/message/iterator_output.py
+-rw-r--r--  2.0 unx     2369 b- defN 24-Mar-11 20:02 sieve/server/grpc/message/single_input.py
+-rw-r--r--  2.0 unx     1038 b- defN 24-Feb-12 21:35 sieve/server/grpc/message/single_output.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/handling/__init__.py
+-rw-r--r--  2.0 unx    12669 b- defN 24-Mar-25 21:36 sieve/server/handling/file_handling.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Feb-12 21:35 sieve/server/handling/sys_handling.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/logging/__init__.py
+-rw-r--r--  2.0 unx     5296 b- defN 24-Apr-23 17:56 sieve/server/logging/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/server/proto/__init__.py
+-rw-r--r--  2.0 unx     2588 b- defN 24-Feb-12 21:35 sieve/server/proto/server_pb2.py
+-rw-r--r--  2.0 unx     2307 b- defN 24-Feb-12 21:35 sieve/server/proto/server_pb2.pyi
+-rw-r--r--  2.0 unx     6063 b- defN 24-Feb-12 21:35 sieve/server/proto/server_pb2_grpc.py
+-rw-r--r--  2.0 unx     3589 b- defN 24-Feb-12 21:35 sieve/server/proto/worker_pb2.py
+-rw-r--r--  2.0 unx     3975 b- defN 24-Feb-12 21:35 sieve/server/proto/worker_pb2.pyi
+-rw-r--r--  2.0 unx     6122 b- defN 24-Feb-12 21:35 sieve/server/proto/worker_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 21:35 sieve/types/__init__.py
+-rw-r--r--  2.0 unx      635 b- defN 24-Mar-25 19:36 sieve/types/base.py
+-rw-r--r--  2.0 unx    26598 b- defN 24-Apr-15 18:36 sieve/types/file.py
+-rw-r--r--  2.0 unx      333 b- defN 24-Mar-25 19:36 sieve/types/metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 19:35 sieve/workflows/__init__.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Mar-25 19:36 sieve/workflows/config.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Mar-25 19:35 sieve/workflows/workflow.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      943 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9002 b- defN 24-Apr-23 17:58 sievedata-1.0.7.dist-info/RECORD
+102 files, 647794 bytes uncompressed, 117327 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -1,46 +1,10 @@
-Filename: cli/__init__.py
-Comment: 
-
-Filename: cli/sieve.py
-Comment: 
-
-Filename: cli/commands/__init__.py
-Comment: 
-
-Filename: cli/commands/feedback.py
-Comment: 
-
-Filename: cli/commands/job.py
-Comment: 
-
-Filename: cli/commands/model.py
-Comment: 
-
-Filename: cli/commands/projects.py
-Comment: 
-
-Filename: cli/commands/query.py
-Comment: 
-
-Filename: cli/commands/secret.py
-Comment: 
-
-Filename: cli/commands/weights.py
-Comment: 
-
-Filename: cli/commands/workflow.py
-Comment: 
-
 Filename: sieve/__init__.py
 Comment: 
 
-Filename: sieve/serialization.py
-Comment: 
-
 Filename: sieve/_cli/__init__.py
 Comment: 
 
 Filename: sieve/_cli/sieve.py
 Comment: 
 
 Filename: sieve/_cli/commands/__init__.py
@@ -81,113 +45,44 @@
 
 Filename: sieve/_openapi/api/default_api.py
 Comment: 
 
 Filename: sieve/_openapi/models/__init__.py
 Comment: 
 
-Filename: sieve/_openapi/models/active.py
-Comment: 
-
-Filename: sieve/_openapi/models/awaiting_resources.py
-Comment: 
-
 Filename: sieve/_openapi/models/body_get_upload_url_v1_upload_url_post.py
 Comment: 
 
-Filename: sieve/_openapi/models/built_at.py
-Comment: 
-
-Filename: sieve/_openapi/models/children.py
-Comment: 
-
-Filename: sieve/_openapi/models/code_url.py
-Comment: 
-
-Filename: sieve/_openapi/models/completed_at.py
-Comment: 
-
 Filename: sieve/_openapi/models/config_model.py
 Comment: 
 
-Filename: sieve/_openapi/models/cover_image_url.py
-Comment: 
-
-Filename: sieve/_openapi/models/created_at.py
-Comment: 
-
-Filename: sieve/_openapi/models/cuda_version.py
-Comment: 
-
-Filename: sieve/_openapi/models/data.py
-Comment: 
-
-Filename: sieve/_openapi/models/default.py
-Comment: 
-
-Filename: sieve/_openapi/models/description.py
-Comment: 
-
-Filename: sieve/_openapi/models/description1.py
-Comment: 
-
-Filename: sieve/_openapi/models/description2.py
-Comment: 
-
-Filename: sieve/_openapi/models/end_timestamp.py
-Comment: 
-
-Filename: sieve/_openapi/models/env.py
-Comment: 
-
 Filename: sieve/_openapi/models/environment_variable.py
 Comment: 
 
-Filename: sieve/_openapi/models/environment_variables.py
-Comment: 
-
-Filename: sieve/_openapi/models/error.py
-Comment: 
-
-Filename: sieve/_openapi/models/featured_key.py
-Comment: 
-
 Filename: sieve/_openapi/models/function.py
 Comment: 
 
 Filename: sieve/_openapi/models/function_app.py
 Comment: 
 
-Filename: sieve/_openapi/models/function_type.py
-Comment: 
-
 Filename: sieve/_openapi/models/http_validation_error.py
 Comment: 
 
-Filename: sieve/_openapi/models/id.py
-Comment: 
-
 Filename: sieve/_openapi/models/id_response.py
 Comment: 
 
-Filename: sieve/_openapi/models/idle.py
-Comment: 
-
 Filename: sieve/_openapi/models/input_output.py
 Comment: 
 
 Filename: sieve/_openapi/models/inputs.py
 Comment: 
 
 Filename: sieve/_openapi/models/job.py
 Comment: 
 
-Filename: sieve/_openapi/models/job_function.py
-Comment: 
-
 Filename: sieve/_openapi/models/job_outputs_inner.py
 Comment: 
 
 Filename: sieve/_openapi/models/list_function_jobs_response.py
 Comment: 
 
 Filename: sieve/_openapi/models/list_response_job.py
@@ -195,122 +90,56 @@
 
 Filename: sieve/_openapi/models/list_response_secret.py
 Comment: 
 
 Filename: sieve/_openapi/models/location_inner.py
 Comment: 
 
-Filename: sieve/_openapi/models/maximum_replicas.py
-Comment: 
-
-Filename: sieve/_openapi/models/model_schema.py
-Comment: 
-
-Filename: sieve/_openapi/models/name.py
-Comment: 
-
 Filename: sieve/_openapi/models/organization_model.py
 Comment: 
 
-Filename: sieve/_openapi/models/outputs.py
-Comment: 
-
 Filename: sieve/_openapi/models/push_request.py
 Comment: 
 
 Filename: sieve/_openapi/models/push_response.py
 Comment: 
 
-Filename: sieve/_openapi/models/queued_at.py
-Comment: 
-
-Filename: sieve/_openapi/models/readme.py
-Comment: 
-
-Filename: sieve/_openapi/models/ready_at.py
-Comment: 
-
-Filename: sieve/_openapi/models/run_id.py
-Comment: 
-
 Filename: sieve/_openapi/models/secret.py
 Comment: 
 
-Filename: sieve/_openapi/models/setup.py
-Comment: 
-
-Filename: sieve/_openapi/models/start_timestamp.py
-Comment: 
-
-Filename: sieve/_openapi/models/started_at.py
-Comment: 
-
-Filename: sieve/_openapi/models/starting.py
-Comment: 
-
 Filename: sieve/_openapi/models/status_response.py
 Comment: 
 
-Filename: sieve/_openapi/models/stream_output.py
-Comment: 
-
-Filename: sieve/_openapi/models/tags.py
-Comment: 
-
-Filename: sieve/_openapi/models/type.py
-Comment: 
-
 Filename: sieve/_openapi/models/upload_model.py
 Comment: 
 
 Filename: sieve/_openapi/models/upload_url_response.py
 Comment: 
 
 Filename: sieve/_openapi/models/user_model.py
 Comment: 
 
 Filename: sieve/_openapi/models/validation_error.py
 Comment: 
 
-Filename: sieve/_openapi/models/validation_error_loc_inner.py
-Comment: 
-
 Filename: sieve/_openapi/models/version.py
 Comment: 
 
-Filename: sieve/_openapi/models/version_current_workers.py
-Comment: 
-
 Filename: sieve/_openapi/models/webhook_model.py
 Comment: 
 
-Filename: sieve/_openapi/models/webhooks.py
-Comment: 
-
-Filename: sieve/_openapi/models/webhooks1.py
-Comment: 
-
 Filename: sieve/_openapi/models/worker_counts.py
 Comment: 
 
-Filename: sieve/_openapi/models/workflow_id.py
-Comment: 
-
 Filename: sieve/_openapi/test/__init__.py
 Comment: 
 
 Filename: sieve/api/__init__.py
 Comment: 
 
-Filename: sieve/api/auth.py
-Comment: 
-
-Filename: sieve/api/client.py
-Comment: 
-
 Filename: sieve/api/common.py
 Comment: 
 
 Filename: sieve/api/constants.py
 Comment: 
 
 Filename: sieve/api/utils.py
@@ -336,86 +165,26 @@
 
 Filename: sieve/api/workflows/__init__.py
 Comment: 
 
 Filename: sieve/api/workflows/common.py
 Comment: 
 
-Filename: sieve/api_v12/__init__.py
-Comment: 
-
-Filename: sieve/api_v12/auth.py
-Comment: 
-
-Filename: sieve/api_v12/client.py
-Comment: 
-
-Filename: sieve/api_v12/common.py
-Comment: 
-
-Filename: sieve/api_v12/constants.py
-Comment: 
-
-Filename: sieve/api_v12/utils.py
-Comment: 
-
-Filename: sieve/api_v12/jobs/__init__.py
-Comment: 
-
-Filename: sieve/api_v12/jobs/common.py
-Comment: 
-
-Filename: sieve/api_v12/models/__init__.py
-Comment: 
-
-Filename: sieve/api_v12/models/common.py
-Comment: 
-
-Filename: sieve/api_v12/secrets/__init__.py
-Comment: 
-
-Filename: sieve/api_v12/secrets/common.py
-Comment: 
-
-Filename: sieve/api_v12/workflows/__init__.py
-Comment: 
-
-Filename: sieve/api_v12/workflows/common.py
-Comment: 
-
 Filename: sieve/functions/__init__.py
 Comment: 
 
-Filename: sieve/functions/common.py
-Comment: 
-
 Filename: sieve/functions/function.py
 Comment: 
 
-Filename: sieve/functions/helpers.py
-Comment: 
-
 Filename: sieve/functions/reference.py
 Comment: 
 
 Filename: sieve/functions/utils.py
 Comment: 
 
-Filename: sieve/predictors/__init__.py
-Comment: 
-
-Filename: sieve/predictors/predictors.py
-Comment: 
-
-Filename: sieve/predictors/trainable.py
-Comment: 
-
-Filename: sieve/predictors/utils.py
-Comment: 
-
 Filename: sieve/server/__init__.py
 Comment: 
 
 Filename: sieve/server/env/__init__.py
 Comment: 
 
 Filename: sieve/server/env/env.py
@@ -498,20 +267,14 @@
 
 Filename: sieve/types/__init__.py
 Comment: 
 
 Filename: sieve/types/base.py
 Comment: 
 
-Filename: sieve/types/box.py
-Comment: 
-
-Filename: sieve/types/embedding.py
-Comment: 
-
 Filename: sieve/types/file.py
 Comment: 
 
 Filename: sieve/types/metadata.py
 Comment: 
 
 Filename: sieve/workflows/__init__.py
@@ -519,26 +282,26 @@
 
 Filename: sieve/workflows/config.py
 Comment: 
 
 Filename: sieve/workflows/workflow.py
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/LICENSE.md
+Filename: sievedata-1.0.7.dist-info/LICENSE.md
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/METADATA
+Filename: sievedata-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/WHEEL
+Filename: sievedata-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/entry_points.txt
+Filename: sievedata-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/top_level.txt
+Filename: sievedata-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: sievedata-1.0.6.dist-info/RECORD
+Filename: sievedata-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sieve/_cli/sieve.py

```diff
@@ -31,15 +31,15 @@
 
 cli = typer.Typer(
     help="Sieve CLI", pretty_exceptions_show_locals=False, invoke_without_command=True
 )
 
 
 def find_sieve_decorator(obj: ast.stmt):
-    if not isinstance(obj, ast.FunctionDef):
+    if not (isinstance(obj, ast.FunctionDef) or isinstance(obj, ast.ClassDef)):
         return False
     for dec in obj.decorator_list:
         if (
             isinstance(dec, ast.Call)
             and isinstance(dec.func, ast.Attribute)
             and isinstance(dec.func.value, ast.Name)
             and dec.func.value.id == "sieve"
```

## sieve/api/common.py

```diff
@@ -155,15 +155,15 @@
         tmp_config["type"] = "function"
         tmp_config["run"] = a.run_commands
         tmp_config["env"] = get_env_list_dict(a.environment_variables)
         tmp_config["public_data"] = process_metadata(a.metadata, api_key)
         tmp_config["restart_on_error"] = a.restart_on_error
         if a.machine_type and isinstance(a.machine_type, str):
             tmp_config["machine_type"] = a.machine_type
-            tmp_config["gpu"] = str(a.gpu != "cpu" and a.gpu != "cpu-ondemand").lower()
+            tmp_config["gpu"] = str(a.machine_type != "cpu" and a.machine_type != "cpu-ondemand").lower()
             tmp_config["split"] = 1
         elif a.machine_type and isinstance(a.machine_type, gpu):
             gpu_type = a.machine_type.gpu if a.machine_type.gpu is not None else "cpu"
             tmp_config["machine_type"] = gpu_type
             tmp_config["gpu"] = str(gpu_type != "cpu").lower()
             tmp_config["split"] = a.machine_type.split
         elif a.gpu and isinstance(a.gpu, gpu):
@@ -206,15 +206,15 @@
         tmp_config["type"] = "model"
         tmp_config["run"] = a.function.run_commands
         tmp_config["env"] = get_env_list_dict(a.environment_variables)
         tmp_config["public_data"] = process_metadata(a.metadata, api_key)
         tmp_config["restart_on_error"] = a.restart_on_error
         if a.machine_type and isinstance(a.machine_type, str):
             tmp_config["machine_type"] = a.machine_type
-            tmp_config["gpu"] = str(a.gpu != "cpu" and a.gpu != "cpu-ondemand").lower()
+            tmp_config["gpu"] = str(a.machine_type != "cpu" and a.machine_type != "cpu-ondemand").lower()
             tmp_config["split"] = 1
         elif a.machine_type and isinstance(a.machine_type, gpu):
             gpu_type = a.machine_type.gpu if a.machine_type.gpu is not None else "cpu"
             tmp_config["machine_type"] = gpu_type
             tmp_config["gpu"] = str(gpu_type != "cpu").lower()
             tmp_config["split"] = a.machine_type.split
         elif a.gpu and isinstance(a.gpu, gpu):
```

## Comparing `sievedata-1.0.6.dist-info/METADATA` & `sievedata-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sievedata
-Version: 1.0.6
+Version: 1.0.7
 Summary: Sieve CLI and Python Client
 Home-page: https://github.com/sieve-data/sieve
 Author: Sieve Team
 Author-email: developer@sievedata.com
 License: unlicensed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

