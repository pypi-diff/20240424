# Comparing `tmp/cognee-0.1.3.tar.gz` & `tmp/cognee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.3.tar", max compression
+gzip compressed data, was "cognee-0.1.4.tar", max compression
```

## Comparing `cognee-0.1.3.tar` & `cognee-0.1.4.tar`

### file list

```diff
@@ -1,155 +1,155 @@
--rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.3/LICENSE
--rw-r--r--   0        0        0     3449 2024-04-21 20:11:09.838701 cognee-0.1.3/README.md
--rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.3/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.3/cognee/api/__init__.py
--rw-r--r--   0        0        0     3242 2024-03-30 16:41:17.062218 cognee-0.1.3/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.3/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.3/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     4642 2024-04-21 19:40:11.051001 cognee-0.1.3/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.3/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.3/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0     6629 2024-04-20 17:06:04.931686 cognee-0.1.3/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.3/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0     2128 2024-04-20 17:06:04.932458 cognee-0.1.3/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.3/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.3/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.3/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.3/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3534 2024-04-20 17:45:58.021645 cognee-0.1.3/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0     6290 2024-04-20 17:16:57.816028 cognee-0.1.3/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.3/cognee/fetch_secret.py
--rw-r--r--   0        0        0     7242 2024-04-20 17:28:06.014788 cognee-0.1.3/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.3/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.3/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.3/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.3/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.3/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.3/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.3/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.3/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.3/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-20 17:13:59.861624 cognee-0.1.3/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.3/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.3/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
--rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.3/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.3/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     5212 2024-04-20 17:06:04.936777 cognee-0.1.3/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.3/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.3/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.3/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.3/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.3/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.3/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.3/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.3/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.3/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      261 2024-04-20 17:06:04.938241 cognee-0.1.3/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.3/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.3/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.3/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6114 2024-04-20 17:06:04.938634 cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.3/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     4664 2024-04-20 17:37:59.594359 cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.3/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.3/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.3/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.3/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.3/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.3/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.3/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-03-29 13:33:11.690414 cognee-0.1.3/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0      835 2024-03-29 12:58:54.566704 cognee-0.1.3/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.3/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.3/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.3/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.3/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.3/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.3/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.3/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.3/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.3/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.3/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.3/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.3/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.3/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.3/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.3/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.3/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.3/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353900 cognee-0.1.3/cognee/infrastructure/pipeline/models/_init_.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.3/cognee/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.3/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.3/cognee/modules/cognify/dataset.py
--rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.3/cognee/modules/cognify/evaluate.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.3/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1186 2024-04-20 17:06:04.943347 cognee-0.1.3/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     4928 2024-04-21 19:46:17.929629 cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
--rw-r--r--   0        0        0      915 2024-04-20 17:06:04.943871 cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layers.py
--rw-r--r--   0        0        0     1265 2024-04-20 17:06:04.944165 cognee-0.1.3/cognee/modules/cognify/graph/add_data_chunks.py
--rw-r--r--   0        0        0      797 2024-04-20 17:06:04.944492 cognee-0.1.3/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     1948 2024-04-20 17:06:04.944822 cognee-0.1.3/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.3/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0      798 2024-04-20 17:06:04.945404 cognee-0.1.3/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.3/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.3/cognee/modules/cognify/graph/initialize_graph.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.3/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.3/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.3/cognee/modules/cognify/test.py
--rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.3/cognee/modules/cognify/train.py
--rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.3/cognee/modules/data/extraction/extract_categories.py
--rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.3/cognee/modules/data/extraction/extract_cognitive_layers.py
--rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.3/cognee/modules/data/extraction/extract_summary.py
--rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
--rw-r--r--   0        0        0     1102 2024-04-20 17:06:04.948874 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
--rw-r--r--   0        0        0     4726 2024-04-20 18:13:47.472889 cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
--rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.3/cognee/modules/data/get_cognitive_layers.py
--rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.3/cognee/modules/data/get_content_categories.py
--rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.3/cognee/modules/data/get_content_summary.py
--rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.3/cognee/modules/data/get_layer_graphs.py
--rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.3/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.3/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.3/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.3/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0     8775 2024-04-20 17:06:04.950504 cognee-0.1.3/cognee/modules/ingestion/chunkers.py
--rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.3/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.3/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.3/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.3/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.3/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.3/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.3/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.3/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.3/cognee/modules/memory/__init__.py
--rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.3/cognee/modules/memory/vector/__init__.py
--rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.3/cognee/modules/memory/vector/create_vector_memory.py
--rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.3/cognee/modules/search/CogneeSearch.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.3/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.3/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.3/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.3/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.3/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.3/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.3/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.3/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.3/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.3/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.3/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.3/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.3/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.3/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
--rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.3/cognee/root_dir.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.3/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8681 2024-04-20 17:06:04.953716 cognee-0.1.3/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.3/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0     5635 2024-04-20 17:06:04.953913 cognee-0.1.3/cognee/tests/test_library.py
--rw-r--r--   0        0        0     8721 2024-04-21 19:46:01.389886 cognee-0.1.3/cognee/utils.py
--rw-r--r--   0        0        0     3472 2024-04-21 20:10:30.296961 cognee-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6882 1970-01-01 00:00:00.000000 cognee-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3668 2024-04-24 17:34:59.318133 cognee-0.1.4/README.md
+-rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.4/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.4/cognee/api/__init__.py
+-rw-r--r--   0        0        0     3242 2024-03-30 16:41:17.062218 cognee-0.1.4/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.4/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.4/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     4719 2024-04-24 17:34:59.318599 cognee-0.1.4/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.4/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.4/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0     6957 2024-04-24 17:34:59.318939 cognee-0.1.4/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.4/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.4/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.4/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.4/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.4/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.4/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3612 2024-04-24 17:34:59.319907 cognee-0.1.4/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0     6471 2024-04-24 17:34:59.320284 cognee-0.1.4/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.4/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     7858 2024-04-24 17:34:59.320914 cognee-0.1.4/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.4/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.4/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.4/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.4/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.4/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.4/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.4/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.4/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.4/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.4/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-20 17:13:59.861624 cognee-0.1.4/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.4/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5212 2024-04-20 17:06:04.936777 cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.4/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.4/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.4/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.4/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.4/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.4/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.4/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.4/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.4/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      261 2024-04-20 17:06:04.938241 cognee-0.1.4/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.4/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.4/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.4/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6114 2024-04-20 17:06:04.938634 cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     2195 2024-03-29 12:58:54.565755 cognee-0.1.4/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4664 2024-04-20 17:37:59.594359 cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.4/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.4/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.4/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.4/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.4/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.4/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.4/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.4/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.4/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.4/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.4/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.4/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.4/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.4/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.4/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.4/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.4/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.4/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.4/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.4/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.4/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.4/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.4/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.4/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.4/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.4/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353900 cognee-0.1.4/cognee/infrastructure/pipeline/models/_init_.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.4/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.4/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.4/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.4/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.4/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1186 2024-04-24 17:35:40.798253 cognee-0.1.4/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     4928 2024-04-24 17:35:40.798450 cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0      915 2024-04-24 17:35:40.798631 cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     1273 2024-04-24 17:34:59.322096 cognee-0.1.4/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0      797 2024-04-24 17:35:40.798810 cognee-0.1.4/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     1948 2024-04-24 17:35:40.798974 cognee-0.1.4/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.4/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      798 2024-04-24 17:35:40.799140 cognee-0.1.4/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.4/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.4/cognee/modules/cognify/graph/initialize_graph.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.4/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.4/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.4/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.4/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.4/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.4/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.4/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1102 2024-04-24 17:35:40.799380 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4726 2024-04-24 17:35:40.799590 cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.4/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.4/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.4/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.4/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.4/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.4/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.4/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.4/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.4/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.4/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.4/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.4/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.4/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.4/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.4/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.4/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.360307 cognee-0.1.4/cognee/modules/memory/__init__.py
+-rw-r--r--   0        0        0       55 2024-03-13 17:10:40.361059 cognee-0.1.4/cognee/modules/memory/vector/__init__.py
+-rw-r--r--   0        0        0      378 2024-03-13 17:10:40.361283 cognee-0.1.4/cognee/modules/memory/vector/create_vector_memory.py
+-rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.4/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.4/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.4/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.4/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.4/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.4/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.4/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.4/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.4/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.4/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.4/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.4/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.4/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.4/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.4/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.4/cognee/root_dir.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.4/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-24 17:35:40.799838 cognee-0.1.4/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.4/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0     5635 2024-04-20 17:06:04.953913 cognee-0.1.4/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     9360 2024-04-24 17:34:59.322831 cognee-0.1.4/cognee/utils.py
+-rw-r--r--   0        0        0     3491 2024-04-24 17:36:10.281347 cognee-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 cognee-0.1.4/PKG-INFO
```

### Comparing `cognee-0.1.3/LICENSE` & `cognee-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/README.md` & `cognee-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,20 @@
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
 ![Cognee Demo](assets/cognee_demo.gif)
 
-For more details, have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+Try it in a Google collab  <a href="https://colab.research.google.com/drive/11k0GtbrKRVGTxhcgad4Wl8YvCnWJVWPl?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+
+Join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
+
+
+
 
 
 ## 📦 Installation
 
 With pip:
 
 ```bash
@@ -67,15 +72,15 @@
 
 ```
 import cognee
 
 text = """Natural language processing (NLP) is an interdisciplinary
        subfield of computer science and information retrieval"""
 
-cognee.add(text) # Add a new piece of information
+cognee.add([text], "example_dataset") # Add a new piece of information
 
 cognee.cognify() # Use LLMs and cognee to create knowledge
 
 search_results = cognee.search("SIMILARITY", "computer science") # Query cognee for the knowledge
 
 for result_text in search_results[0]:
     print(result_text)
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
 # cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
 vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
-![Cognee Demo](assets/cognee_demo.gif) For more details, have a look at our
-_d_o_c_u_m_e_n_t_a_t_i_o_n ## ð¦ Installation With pip: ```bash pip install "cognee
-[weaviate]" ``` With poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð»
-Usage ### Setup ``` import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
-os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ
-["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama or
-Anyscale as your LLM provider. For more info on local models check our [docs]
-(https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
-"""Natural language processing (NLP) is an interdisciplinary subfield of
-computer science and information retrieval""" cognee.add(text) # Add a new
-piece of information cognee.cognify() # Use LLMs and cognee to create knowledge
-search_results = cognee.search("SIMILARITY", "computer science") # Query cognee
-for the knowledge for result_text in search_results[0]: print(result_text) ```
-Add alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
+![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
+have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
+Installation With pip: ```bash pip install "cognee[weaviate]" ``` With poetry:
+```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ``` import os
+os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"]
+= "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+``` You can also use Ollama or Anyscale as your LLM provider. For more info on
+local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
+import cognee text = """Natural language processing (NLP) is an
+interdisciplinary subfield of computer science and information retrieval"""
+cognee.add([text], "example_dataset") # Add a new piece of information
+cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
+cognee.search("SIMILARITY", "computer science") # Query cognee for the
+knowledge for result_text in search_results[0]: print(result_text) ``` Add
+alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
 dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
 dataset_name) # This is useful if you have a directory with files organized in
 subdirectories. # You can target which directory to add by providing
 dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
 cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
 just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
 Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
```

### Comparing `cognee-0.1.3/cognee/api/client.py` & `cognee-0.1.4/cognee/api/client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/api/v1/add/add.py` & `cognee-0.1.4/cognee/api/v1/add/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import dlt
 import duckdb
 import cognee.modules.ingestion as ingestion
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.files.storage import LocalStorage
 from cognee.modules.discovery import discover_directory_datasets
 
+from cognee.utils import send_telemetry
+
+
+
 async def add(data_path: Union[str, List[str]], dataset_name: str = None):
     if isinstance(data_path, str):
         # data_path is a data directory path
         if "data://" in data_path:
             return await add_data_directory(data_path.replace("data://", ""), dataset_name)
         # data_path is a file path
         if "file://" in data_path:
@@ -51,15 +55,15 @@
     processed_file_paths = []
 
     for file_path in file_paths:
         file_path = file_path.replace("file://", "")
 
         if data_directory_path not in file_path:
             file_name = file_path.split("/")[-1]
-            file_directory_path = data_directory_path + "/" + (dataset_name.replace('.', "/") + "/" if dataset_name != "root" else "")
+            file_directory_path = data_directory_path + "/" + (dataset_name.replace(".", "/") + "/" if dataset_name != "root" else "")
             dataset_file_path = path.join(file_directory_path, file_name)
 
             LocalStorage.ensure_directory_exists(file_directory_path)
 
             LocalStorage.copy_file(file_path, dataset_file_path)
             processed_file_paths.append(dataset_file_path)
         else:
@@ -97,14 +101,15 @@
 
     run_info = pipeline.run(
         data_resources(processed_file_paths),
         table_name = "file_metadata",
         dataset_name = dataset_name.replace(" ", "_").replace(".", "_") if dataset_name is not None else "main_dataset",
         write_disposition = "merge",
     )
+    send_telemetry( "COGNEE_ADD")
 
     return run_info
 
 async def add_data_directory(data_path: str, dataset_name: str = None):
     datasets = discover_directory_datasets(data_path)
 
     results = []
```

### Comparing `cognee-0.1.3/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.4/cognee/api/v1/add/add_standalone.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/api/v1/add/remember.py` & `cognee-0.1.4/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.4/cognee/api/v1/cognify/cognify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import asyncio
+from uuid import uuid4
 from typing import List, Union
 import logging
 import instructor
 from openai import OpenAI
+from nltk.corpus import stopwords
+from cognee.config import Config
 from cognee.modules.cognify.graph.add_data_chunks import add_data_chunks
 from cognee.modules.cognify.graph.add_document_node import add_document_node
 from cognee.modules.cognify.graph.add_classification_nodes import add_classification_nodes
 from cognee.modules.cognify.graph.add_cognitive_layer_graphs import add_cognitive_layer_graphs
 from cognee.modules.cognify.graph.add_summary_nodes import add_summary_nodes
 from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, \
     graph_ready_output, connect_nodes_in_graph
 from cognee.modules.cognify.llm.resolve_cross_graph_references import resolve_cross_graph_references
-
-from cognee.config import Config
-
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
 from cognee.modules.cognify.graph.add_cognitive_layers import add_cognitive_layers
 # from cognee.modules.cognify.graph.initialize_graph import initialize_graph
 from cognee.infrastructure.files.utils.guess_file_type import guess_file_type, FileTypeException
 from cognee.infrastructure.files.utils.extract_text_from_file import extract_text_from_file
 from cognee.infrastructure import infrastructure_config
 from cognee.modules.data.get_content_categories import get_content_categories
 from cognee.modules.data.get_content_summary import get_content_summary
 from cognee.modules.data.get_cognitive_layers import get_cognitive_layers
 from cognee.modules.data.get_layer_graphs import get_layer_graphs
+from cognee.utils import send_telemetry
+
 
 config = Config()
 config.load()
 
 aclient = instructor.patch(OpenAI())
 
 USER_ID = "default_user"
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("cognify")
 
 async def cognify(datasets: Union[str, List[str]] = None):
     """This function is responsible for the cognitive processing of the content."""
+    # Has to be loaded in advance, multithreading doesn't work without it.
+    stopwords.ensure_loaded()
 
     db_engine = infrastructure_config.get_config()["database_engine"]
 
     if datasets is None or len(datasets) == 0:
         datasets = db_engine.get_datasets()
 
     awaitables = []
@@ -49,18 +53,18 @@
     if isinstance(datasets, list):
         for dataset in datasets:
             awaitables.append(cognify(dataset))
 
         graphs = await asyncio.gather(*awaitables)
         return graphs[0]
 
-    # datasets is a dataset name string
     added_datasets = db_engine.get_datasets()
 
     dataset_files = []
+    # datasets is a dataset name string
     dataset_name = datasets.replace(".", "_").replace(" ", "_")
 
     for added_dataset in added_datasets:
         if dataset_name in added_dataset:
             dataset_files.append((added_dataset, db_engine.get_files_metadata(added_dataset)))
 
     awaitables = []
@@ -69,38 +73,43 @@
 
     graph_client = await get_graph_client(graph_db_type)
 
     # await initialize_graph(USER_ID, graph_data_model, graph_client)
 
     data_chunks = {}
 
+    chunk_engine = infrastructure_config.get_config()["chunk_engine"]
+    chunk_strategy = infrastructure_config.get_config()["chunk_strategy"]
+
     for (dataset_name, files) in dataset_files:
-        for file_metadata in files[:3]:
+        for file_metadata in files:
             with open(file_metadata["file_path"], "rb") as file:
                 try:
                     file_type = guess_file_type(file)
                     text = extract_text_from_file(file, file_type)
+                    subchunks = chunk_engine.chunk_data(chunk_strategy, text, config.chunk_size, config.chunk_overlap)
 
                     if dataset_name not in data_chunks:
                         data_chunks[dataset_name] = []
 
-                    data_chunks[dataset_name].append(dict(text = text, file_metadata = file_metadata))
+                    for subchunk in subchunks:
+                        data_chunks[dataset_name].append(dict(text = subchunk, chunk_id = str(uuid4()), file_metadata = file_metadata))
                 except FileTypeException:
                     logger.warning("File (%s) has an unknown file type. We are skipping it.", file_metadata["id"])
 
     added_chunks: list[tuple[str, str, dict]] = await add_data_chunks(data_chunks)
 
     await asyncio.gather(
-        *[process_text(chunk["collection"], chunk["id"], chunk["text"], chunk["file_metadata"]) for chunk in added_chunks]
+        *[process_text(chunk["collection"], chunk["chunk_id"], chunk["text"], chunk["file_metadata"]) for chunk in added_chunks]
     )
 
     return graph_client.graph
 
 async def process_text(chunk_collection: str, chunk_id: str, input_text: str, file_metadata: dict):
-    print(f"Processing document ({file_metadata['id']}).")
+    print(f"Processing chunk ({chunk_id}) from document ({file_metadata['id']}).")
 
     graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
 
     document_id = await add_document_node(
         graph_client,
         parent_node_id = f"DefaultGraphModel__{USER_ID}", #make a param of defaultgraph model to make sure when user passes his stuff, it doesn't break pipeline
         document_metadata = file_metadata,
@@ -111,53 +120,49 @@
     classified_categories = await get_content_categories(input_text)
     await add_classification_nodes(
         graph_client,
         parent_node_id = document_id,
         categories = classified_categories,
     )
 
-    print(f"Document ({document_id}) classified.")
+    print(f"Chunk ({chunk_id}) classified.")
 
     content_summary = await get_content_summary(input_text)
     await add_summary_nodes(graph_client, document_id, content_summary)
 
-    print(f"Document ({document_id}) summarized.")
+    print(f"Chunk ({chunk_id}) summarized.")
 
     cognitive_layers = await get_cognitive_layers(input_text, classified_categories)
     cognitive_layers = (await add_cognitive_layers(graph_client, document_id, cognitive_layers))[:2]
 
     layer_graphs = await get_layer_graphs(input_text, cognitive_layers)
     await add_cognitive_layer_graphs(graph_client, chunk_collection, chunk_id, layer_graphs)
 
     if infrastructure_config.get_config()["connect_documents"] is True:
         db_engine = infrastructure_config.get_config()["database_engine"]
         relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = file_metadata["id"])
 
-        print("Relevant documents to connect are: ", relevant_documents_to_connect)
-
         list_of_nodes = []
 
         relevant_documents_to_connect.append({
             "layer_id": document_id,
         })
 
         for document in relevant_documents_to_connect:
             node_descriptions_to_match = await graph_client.extract_node_description(document["layer_id"])
             list_of_nodes.extend(node_descriptions_to_match)
 
-        print("List of nodes are: ", len(list_of_nodes))
-
         nodes_by_layer = await group_nodes_by_layer(list_of_nodes)
-        print("Nodes by layer are: ", str(nodes_by_layer)[:5000])
 
         results = await resolve_cross_graph_references(nodes_by_layer)
-        print("Results are: ", str(results)[:3000])
 
         relationships = graph_ready_output(results)
 
         await connect_nodes_in_graph(
             graph_client,
             relationships,
             score_threshold = infrastructure_config.get_config()["intra_layer_score_treshold"]
         )
 
-        print(f"Document ({document_id}) cognified.")
+    send_telemetry( "COGNEE_COGNIFY")
+
+    print(f"Chunk ({chunk_id}) cognified.")
```

### Comparing `cognee-0.1.3/cognee/api/v1/config/config.py` & `cognee-0.1.4/cognee/api/v1/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,8 +63,12 @@
         })
 
     @staticmethod
     def connect_documents(connect_documents: bool):
         infrastructure_config.set_config({
             "connect_documents": connect_documents
         })
-
+    @staticmethod
+    def set_chunk_strategy(chunk_strategy: object):
+        infrastructure_config.set_config({
+            "chunk_strategy": chunk_strategy
+        })
```

### Comparing `cognee-0.1.3/cognee/api/v1/datasets/datasets.py` & `cognee-0.1.4/cognee/api/v1/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/api/v1/prune/prune.py` & `cognee-0.1.4/cognee/api/v1/prune/prune.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/api/v1/search/search.py` & `cognee-0.1.4/cognee/api/v1/search/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from cognee.modules.search.graph.search_adjacent import search_adjacent
 from cognee.modules.search.vector.search_similarity import search_similarity
 from cognee.modules.search.graph.search_categories import search_categories
 from cognee.modules.search.graph.search_neighbour import search_neighbour
 from cognee.modules.search.graph.search_summary import search_summary
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.infrastructure import infrastructure_config
+from cognee.utils import send_telemetry
 
 class SearchType(Enum):
     ADJACENT = 'ADJACENT'
     SIMILARITY = 'SIMILARITY'
     CATEGORIES = 'CATEGORIES'
     NEIGHBOR = 'NEIGHBOR'
     SUMMARY = 'SUMMARY'
@@ -65,14 +66,16 @@
 
     # Use asyncio.gather to run all scheduled tasks concurrently
     search_results = await asyncio.gather(*search_tasks)
 
     # Update the results set with the results from all tasks
     results.extend(search_results)
 
+    send_telemetry( "COGNEE_SEARCH")
+
     return results
 
 
 
 if __name__ == "__main__":
     async def main():
         # Assuming 'graph' is your graph object, obtained from somewhere
```

### Comparing `cognee-0.1.3/cognee/config.py` & `cognee-0.1.4/cognee/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import configparser
 import uuid
 from typing import Optional, Dict, Any
 from dataclasses import dataclass, field
 from pathlib import Path
 from dotenv import load_dotenv
 from cognee.root_dir import get_absolute_path
-
+from cognee.shared.data_models import ChunkStrategy
 
 base_dir = Path(__file__).resolve().parent.parent
 # Load the .env file from the base directory
 dotenv_path = base_dir / ".env"
 load_dotenv(dotenv_path=dotenv_path)
 
 
@@ -112,14 +112,19 @@
     # Model parameters and configuration for interlayer scoring
     intra_layer_score_treshold: float = 0.98
 
 
     # Client ID
     anon_clientid: Optional[str] = field(default_factory=lambda: uuid.uuid4().hex)
 
+    #Chunking parameters
+    chunk_size: int = 1500
+    chunk_overlap: int = 0
+    chunk_strategy: str = ChunkStrategy.PARAGRAPH
+
     def load(self):
         """Loads the configuration from a file or environment variables."""
         config = configparser.ConfigParser()
         config.read(self.config_path)
 
         # Override with environment variables if they exist
         for attr in self.__annotations__:
```

### Comparing `cognee-0.1.3/cognee/fetch_secret.py` & `cognee-0.1.4/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/InfrastructureConfig.py` & `cognee-0.1.4/cognee/infrastructure/InfrastructureConfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .databases.relational import DuckDBAdapter, DatabaseEngine
 from .databases.vector.vector_db_interface import VectorDBInterface
 from .databases.vector.qdrant.QDrantAdapter import QDrantAdapter
 from .databases.vector.embeddings.DefaultEmbeddingEngine import DefaultEmbeddingEngine
 from .llm.llm_interface import LLMInterface
 from .llm.openai.adapter import OpenAIAdapter
 from .files.storage import LocalStorage
+from .data.chunking.DefaultChunkEngine import DefaultChunkEngine
 from ..shared.data_models import GraphDBType, DefaultContentPrediction, KnowledgeGraph, SummarizedContent, \
     LabeledContent, DefaultCognitiveLayer
 
 config = Config()
 config.load()
 
 class InfrastructureConfig():
@@ -26,14 +27,16 @@
     graph_model = None
     cognitive_layer_model = None
     intra_layer_score_treshold = None
     embedding_engine = None
     connect_documents = config.connect_documents
     database_directory_path: str = None
     database_file_path: str = None
+    chunk_strategy = config.chunk_strategy
+    chunk_engine = None
 
     def get_config(self, config_entity: str = None) -> dict:
         if (config_entity is None or config_entity == "database_engine") and self.database_engine is None:
             db_path = self.system_root_directory + "/" + config.db_path
 
             LocalStorage.ensure_directory_exists(db_path)
 
@@ -65,14 +68,20 @@
 
         if self.embedding_engine is None:
             self.embedding_engine = DefaultEmbeddingEngine()
 
         if self.connect_documents is None:
             self.connect_documents = config.connect_documents
 
+        if self.chunk_strategy is None:
+            self.chunk_strategy = config.chunk_strategy
+
+        if self.chunk_engine is None:
+            self.chunk_engine = DefaultChunkEngine()
+
         if (config_entity is None or config_entity == "llm_engine") and self.llm_engine is None:
             self.llm_engine = OpenAIAdapter(config.openai_key, config.openai_model)
 
         if (config_entity is None or config_entity == "vector_engine") and self.vector_engine is None:
             try:
                 from .databases.vector.weaviate_db import WeaviateAdapter
 
@@ -116,24 +125,26 @@
             "graph_model": self.graph_model,
             "cognitive_layer_model": self.cognitive_layer_model,
             "llm_provider": self.llm_provider,
             "intra_layer_score_treshold": self.intra_layer_score_treshold,
             "embedding_engine": self.embedding_engine,
             "connect_documents": self.connect_documents,
             "database_directory_path": self.database_directory_path,
-            "database_path": self.database_file_path
+            "database_path": self.database_file_path,
+            "chunk_strategy": self.chunk_strategy,
+            "chunk_engine": self.chunk_engine,
         }
 
     def set_config(self, new_config: dict):
         if "system_root_directory" in new_config:
             self.system_root_directory = new_config["system_root_directory"]
-      
+
         if "data_root_directory" in new_config:
             self.data_root_directory = new_config["data_root_directory"]
-      
+
         if "database_engine" in new_config:
             self.database_engine = new_config["database_engine"]
 
         if "vector_engine" in new_config:
             self.vector_engine = new_config["vector_engine"]
 
         if "llm_engine" in new_config:
@@ -165,8 +176,14 @@
 
         if "embedding_engine" in new_config:
             self.embedding_engine = new_config["embedding_engine"]
 
         if "connect_documents" in new_config:
             self.connect_documents = new_config["connect_documents"]
 
+        if "chunk_strategy" in new_config:
+            self.chunk_strategy = new_config["chunk_strategy"]
+
+        if "chunk_engine" in new_config:
+            self.chunk_engine = new_config["chunk_engine"]
+
 infrastructure_config = InfrastructureConfig()
```

### Comparing `cognee-0.1.3/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.4/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.4/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.4/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.4/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/graph/get_graph_client.py` & `cognee-0.1.4/cognee/infrastructure/databases/graph/get_graph_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.4/cognee/infrastructure/databases/graph/graph_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py` & `cognee-0.1.4/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/graph/networkx/adapter.py` & `cognee-0.1.4/cognee/infrastructure/databases/graph/networkx/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py` & `cognee-0.1.4/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.4/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.4/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.4/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py` & `cognee-0.1.4/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.4/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.4/cognee/infrastructure/databases/vector/vector_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.4/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.4/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.4/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.4/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/files/utils/guess_file_type.py` & `cognee-0.1.4/cognee/infrastructure/files/utils/guess_file_type.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.4/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.4/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.4/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/get_llm_client.py` & `cognee-0.1.4/cognee/infrastructure/llm/get_llm_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/llm_interface.py` & `cognee-0.1.4/cognee/infrastructure/llm/llm_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.4/cognee/infrastructure/llm/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.4/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.4/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.4/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.4/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.4/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/dataset.py` & `cognee-0.1.4/cognee/modules/cognify/dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/evaluate.py` & `cognee-0.1.4/cognee/modules/cognify/evaluate.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_classification_nodes.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_classification_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_cognitive_layers.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_data_chunks.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_data_chunks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TypedDict
-from uuid import uuid4
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.vector import DataPoint
 
 class TextChunk(TypedDict):
     text: str
+    chunk_id: str
     file_metadata: dict
 
 async def add_data_chunks(dataset_data_chunks: dict[str, list[TextChunk]]):
     vector_client = infrastructure_config.get_config("vector_engine")
 
     identified_chunks = []
 
@@ -16,28 +16,28 @@
         try:
             await vector_client.create_collection(dataset_name)
         except Exception:
             pass
 
         dataset_chunks = [
             dict(
-                id = str(uuid4()),
+                chunk_id = chunk["chunk_id"],
                 collection = dataset_name,
                 text = chunk["text"],
                 file_metadata = chunk["file_metadata"],
             ) for chunk in chunks
         ]
-    
+
         identified_chunks.extend(dataset_chunks)
 
         await vector_client.create_data_points(
             dataset_name,
             [
                 DataPoint(
-                    id = chunk["id"],
+                    id = chunk["chunk_id"],
                     payload = dict(text = chunk["text"]),
                     embed_field = "text"
                 ) for chunk in dataset_chunks
             ],
         )
 
     return identified_chunks
```

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_document_node.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_document_node.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_label_nodes.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_label_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/add_summary_nodes.py` & `cognee-0.1.4/cognee/modules/cognify/graph/add_summary_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/create.py` & `cognee-0.1.4/cognee/modules/cognify/graph/create.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/graph/initialize_graph.py` & `cognee-0.1.4/cognee/modules/cognify/graph/initialize_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.4/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/test.py` & `cognee-0.1.4/cognee/modules/cognify/test.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/cognify/train.py` & `cognee-0.1.4/cognee/modules/cognify/train.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/extraction/extract_categories.py` & `cognee-0.1.4/cognee/modules/data/extraction/extract_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py` & `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py` & `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py` & `cognee-0.1.4/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/get_cognitive_layers.py` & `cognee-0.1.4/cognee/modules/data/get_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/get_content_categories.py` & `cognee-0.1.4/cognee/modules/data/get_content_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/data/get_layer_graphs.py` & `cognee-0.1.4/cognee/modules/data/get_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.4/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.4/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/ingestion/data_types/BinaryData.py` & `cognee-0.1.4/cognee/modules/ingestion/data_types/BinaryData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/ingestion/data_types/TextData.py` & `cognee-0.1.4/cognee/modules/ingestion/data_types/TextData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/ingestion/save.py` & `cognee-0.1.4/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/CogneeSearch.py` & `cognee-0.1.4/cognee/modules/search/CogneeSearch.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/graph/search_adjacent.py` & `cognee-0.1.4/cognee/modules/search/graph/search_adjacent.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/graph/search_categories.py` & `cognee-0.1.4/cognee/modules/search/graph/search_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/graph/search_neighbour.py` & `cognee-0.1.4/cognee/modules/search/graph/search_neighbour.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/graph/search_summary.py` & `cognee-0.1.4/cognee/modules/search/graph/search_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/search/vector/search_similarity.py` & `cognee-0.1.4/cognee/modules/search/vector/search_similarity.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.4/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json` & `cognee-0.1.4/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/shared/data_models.py` & `cognee-0.1.4/cognee/shared/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     """Answer."""
     answer: str
 
 class ChunkStrategy(Enum):
     EXACT = "exact"
     PARAGRAPH = "paragraph"
     SENTENCE = "sentence"
-    VANILLA = "vanilla"
-    SUMMARY = "summary"
 
 class MemorySummary(BaseModel):
     """ Memory summary. """
     nodes: List[Node] = Field(..., default_factory=list)
     edges: List[Edge] = Field(..., default_factory=list)
```

### Comparing `cognee-0.1.3/cognee/tests/test_library.py` & `cognee-0.1.4/cognee/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.3/cognee/utils.py` & `cognee-0.1.4/cognee/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,42 @@
 import graphistry
 import networkx as nx
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import tiktoken
 import nltk
+from posthog import Posthog
+
 from cognee.config import Config
+import uuid
+import datetime
 
 config = Config()
 config.load()
 
+
+def send_telemetry( posthog, event_name="COGNEE_ADD"):
+    if os.getenv("TELEMETRY_DISABLED"):
+        return
+
+    posthog = Posthog(project_api_key='phc_bbR86N876kwub62Lr3dhQ7zIeRyMMMm0fxXqxPqzLm3',
+                      host='https://eu.i.posthog.com')
+
+    user_id = str(uuid.uuid4())
+    current_time = datetime.datetime.now()
+    properties = {
+        "time": current_time.strftime('%m/%d/%Y')
+
+    }
+
+    try:
+        posthog.capture(user_id, event_name, properties)
+    except Exception as e:
+        print('ERROR sending telemetric data to Posthog. See exception: %s', e)
 def get_document_names(doc_input):
     """
     Get a list of document names.
 
     This function takes doc_input, which can be a folder path,
     a single document file path, or a document name as a string.
     It returns a list of document names based on the doc_input.
```

### Comparing `cognee-0.1.3/pyproject.toml` & `cognee-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.3"
+version = "0.1.4"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
 authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
@@ -57,14 +57,15 @@
 neo4j = "^5.18.0"
 jinja2 = "^3.1.3"
 matplotlib = "^3.8.3"
 nest-asyncio = "^1.6.0"
 structlog = "^24.1.0"
 tiktoken = "^0.6.0"
 dspy-ai = "2.4.3"
+posthog = "^3.5.0"
 
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake", "dbt-athena-community", "dbt-databricks"]
 gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
 bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
```

### Comparing `cognee-0.1.3/PKG-INFO` & `cognee-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -63,14 +63,15 @@
 Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
+Requires-Dist: posthog (>=3.5.0,<4.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse"
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.0.3,<4.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: qdrant-client (>=1.8.0,<2.0.0)
 Requires-Dist: ruff (>=0.2.2,<0.3.0)
@@ -114,15 +115,20 @@
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
 ![Cognee Demo](assets/cognee_demo.gif)
 
-For more details, have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+Try it in a Google collab  <a href="https://colab.research.google.com/drive/11k0GtbrKRVGTxhcgad4Wl8YvCnWJVWPl?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+
+Join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
+
+
+
 
 
 ## 📦 Installation
 
 With pip:
 
 ```bash
@@ -154,15 +160,15 @@
 
 ```
 import cognee
 
 text = """Natural language processing (NLP) is an interdisciplinary
        subfield of computer science and information retrieval"""
 
-cognee.add(text) # Add a new piece of information
+cognee.add([text], "example_dataset") # Add a new piece of information
 
 cognee.cognify() # Use LLMs and cognee to create knowledge
 
 search_results = cognee.search("SIMILARITY", "computer science") # Query cognee for the knowledge
 
 for result_text in search_results[0]:
     print(result_text)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.3 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.4 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
 2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
@@ -28,45 +28,47 @@
 graphviz (>=0.20.1,<0.21.0) Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-
 Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-
 Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j" Requires-Dist: nest-
 asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0) Requires-
 Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-Dist:
 overrides (>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas
-(>=2.2.0,<3.0.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra ==
-"bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena"
-or extra == "synapse" Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-Dist:
-pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf (>=4.1.0,<5.0.0) Requires-Dist:
-python-dotenv (==1.0.1) Requires-Dist: qdrant-client (>=1.8.0,<2.0.0) Requires-
-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0) Requires-Dist: structlog
-(>=24.1.0,<25.0.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist:
-tiktoken (>=0.6.0,<0.7.0) Requires-Dist: uvicorn (==0.22.0) Requires-Dist:
-weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate" Requires-Dist: xmltodict
-(>=0.13.0,<0.14.0) Project-URL: Repository, https://github.com/topoteretes/
-cognee Description-Content-Type: text/markdown # cognee Deterministic LLMs
-Outputs for AI Engineers using graphs, LLMs and vector retrieval
+(>=2.2.0,<3.0.0) Requires-Dist: posthog (>=3.5.0,<4.0.0) Requires-Dist: pyarrow
+(>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra ==
+"motherduck" or extra == "athena" or extra == "synapse" Requires-Dist: pydantic
+(>=2.5.0,<3.0.0) Requires-Dist: pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf
+(>=4.1.0,<5.0.0) Requires-Dist: python-dotenv (==1.0.1) Requires-Dist: qdrant-
+client (>=1.8.0,<2.0.0) Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist:
+scikit-learn (>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tenacity
+(>=8.2.3,<9.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist:
+uvicorn (==0.22.0) Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra ==
+"weaviate" Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository,
+https://github.com/topoteretes/cognee Description-Content-Type: text/markdown #
+cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
+vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
-![Cognee Demo](assets/cognee_demo.gif) For more details, have a look at our
-_d_o_c_u_m_e_n_t_a_t_i_o_n ## ð¦ Installation With pip: ```bash pip install "cognee
-[weaviate]" ``` With poetry: ```bash poetry add "cognee[weaviate]" ``` ## ð»
-Usage ### Setup ``` import os os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
-os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY" os.environ
-["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama or
-Anyscale as your LLM provider. For more info on local models check our [docs]
-(https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
-"""Natural language processing (NLP) is an interdisciplinary subfield of
-computer science and information retrieval""" cognee.add(text) # Add a new
-piece of information cognee.cognify() # Use LLMs and cognee to create knowledge
-search_results = cognee.search("SIMILARITY", "computer science") # Query cognee
-for the knowledge for result_text in search_results[0]: print(result_text) ```
-Add alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
+![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
+have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
+Installation With pip: ```bash pip install "cognee[weaviate]" ``` With poetry:
+```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ``` import os
+os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"]
+= "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+``` You can also use Ollama or Anyscale as your LLM provider. For more info on
+local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
+import cognee text = """Natural language processing (NLP) is an
+interdisciplinary subfield of computer science and information retrieval"""
+cognee.add([text], "example_dataset") # Add a new piece of information
+cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
+cognee.search("SIMILARITY", "computer science") # Query cognee for the
+knowledge for result_text in search_results[0]: print(result_text) ``` Add
+alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
 dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
 dataset_name) # This is useful if you have a directory with files organized in
 subdirectories. # You can target which directory to add by providing
 dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
 cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
 just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
 Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
```

