# Comparing `tmp/embedchain-0.1.98.tar.gz` & `tmp/embedchain-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.1.98.tar", max compression
+gzip compressed data, was "embedchain-0.1.99.tar", max compression
```

## Comparing `embedchain-0.1.98.tar` & `embedchain-0.1.99.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    11349 2024-03-21 02:30:45.585445 embedchain-0.1.98/LICENSE
--rw-r--r--   0        0        0     5650 2024-03-21 02:30:45.585445 embedchain-0.1.98/README.md
--rw-r--r--   0        0        0      313 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/__init__.py
--rw-r--r--   0        0        0     3615 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/alembic.ini
--rw-r--r--   0        0        0    20753 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/app.py
--rw-r--r--   0        0        0      193 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/__init__.py
--rw-r--r--   0        0        0     1636 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/base.py
--rw-r--r--   0        0        0     4335 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/discord.py
--rw-r--r--   0        0        0     3010 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/poe.py
--rw-r--r--   0        0        0     3938 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/slack.py
--rw-r--r--   0        0        0     2689 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/bots/whatsapp.py
--rw-r--r--   0        0        0     1548 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/cache.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/__init__.py
--rw-r--r--   0        0        0     3326 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/base_chunker.py
--rw-r--r--   0        0        0      805 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/beehiiv.py
--rw-r--r--   0        0        0      815 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/common_chunker.py
--rw-r--r--   0        0        0      809 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/discourse.py
--rw-r--r--   0        0        0      813 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/docs_site.py
--rw-r--r--   0        0        0      809 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/docx_file.py
--rw-r--r--   0        0        0      801 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/gmail.py
--rw-r--r--   0        0        0      821 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/google_drive.py
--rw-r--r--   0        0        0      802 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/image.py
--rw-r--r--   0        0        0      799 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/json.py
--rw-r--r--   0        0        0      803 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/mdx.py
--rw-r--r--   0        0        0      800 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/mysql.py
--rw-r--r--   0        0        0      802 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/notion.py
--rw-r--r--   0        0        0      675 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/openapi.py
--rw-r--r--   0        0        0      806 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/pdf_file.py
--rw-r--r--   0        0        0      807 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/postgres.py
--rw-r--r--   0        0        0      805 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/qna_pair.py
--rw-r--r--   0        0        0      806 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/rss_feed.py
--rw-r--r--   0        0        0      804 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/sitemap.py
--rw-r--r--   0        0        0      804 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/slack.py
--rw-r--r--   0        0        0      807 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/substack.py
--rw-r--r--   0        0        0      749 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/table.py
--rw-r--r--   0        0        0      798 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/text.py
--rw-r--r--   0        0        0      824 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/unstructured_file.py
--rw-r--r--   0        0        0      806 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/web_page.py
--rw-r--r--   0        0        0      803 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/xml.py
--rw-r--r--   0        0        0      816 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/chunkers/youtube_video.py
--rw-r--r--   0        0        0    12794 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/cli.py
--rw-r--r--   0        0        0     3275 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/client.py
--rw-r--r--   0        0        0      523 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/__init__.py
--rw-r--r--   0        0        0     2407 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/add_config.py
--rw-r--r--   0        0        0     1282 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/app_config.py
--rw-r--r--   0        0        0     2358 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/base_app_config.py
--rw-r--r--   0        0        0      453 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/base_config.py
--rw-r--r--   0        0        0     3780 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/cache_config.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/embedder/__init__.py
--rw-r--r--   0        0        0      982 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/embedder/base.py
--rw-r--r--   0        0        0      609 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/embedder/google.py
--rw-r--r--   0        0        0      119 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/evaluation/__init__.py
--rw-r--r--   0        0        0     3457 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/evaluation/base.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/llm/__init__.py
--rw-r--r--   0        0        0     8336 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/llm/base.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/__init__.py
--rw-r--r--   0        0        0     1385 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/base.py
--rw-r--r--   0        0        0     1591 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/chroma.py
--rw-r--r--   0        0        0     2438 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/elasticsearch.py
--rw-r--r--   0        0        0     1556 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/opensearch.py
--rw-r--r--   0        0        0     1859 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/pinecone.py
--rw-r--r--   0        0        0     1993 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/qdrant.py
--rw-r--r--   0        0        0      505 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/weaviate.py
--rw-r--r--   0        0        0     2055 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/config/vectordb/zilliz.py
--rw-r--r--   0        0        0      372 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/core/db/__init__.py
--rw-r--r--   0        0        0     3043 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/core/db/database.py
--rw-r--r--   0        0        0      944 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/core/db/models.py
--rw-r--r--   0        0        0       56 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/data_formatter/__init__.py
--rw-r--r--   0        0        0     7743 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/data_formatter/data_formatter.py
--rw-r--r--   0        0        0        3 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/fly.io/.dockerignore
--rw-r--r--   0        0        0       21 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/fly.io/.env.example
--rw-r--r--   0        0        0      195 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/fly.io/Dockerfile
--rw-r--r--   0        0        0     1296 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/fly.io/app.py
--rw-r--r--   0        0        0       58 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/fly.io/requirements.txt
--rw-r--r--   0        0        0      221 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/gradio.app/app.py
--rw-r--r--   0        0        0       26 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/gradio.app/requirements.txt
--rw-r--r--   0        0        0       21 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/modal.com/.env.example
--rw-r--r--   0        0        0        5 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/modal.com/.gitignore
--rw-r--r--   0        0        0     1913 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/modal.com/app.py
--rw-r--r--   0        0        0       61 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/modal.com/requirements.txt
--rw-r--r--   0        0        0       21 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/render.com/.env.example
--rw-r--r--   0        0        0        5 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/render.com/.gitignore
--rw-r--r--   0        0        0     1244 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/render.com/app.py
--rw-r--r--   0        0        0      506 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/render.com/render.yaml
--rw-r--r--   0        0        0       58 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/render.com/requirements.txt
--rw-r--r--   0        0        0       24 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/streamlit.io/.streamlit/secrets.toml
--rw-r--r--   0        0        0     1962 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/streamlit.io/app.py
--rw-r--r--   0        0        0       29 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/deployment/streamlit.io/requirements.txt
--rw-r--r--   0        0        0    29680 2024-03-21 02:30:45.649444 embedchain-0.1.98/embedchain/embedchain.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/__init__.py
--rw-r--r--   0        0        0     3001 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/base.py
--rw-r--r--   0        0        0      738 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/cohere.py
--rw-r--r--   0        0        0     1459 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/google.py
--rw-r--r--   0        0        0      770 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/gpt4all.py
--rw-r--r--   0        0        0      764 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/huggingface.py
--rw-r--r--   0        0        0     1711 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/mistralai.py
--rw-r--r--   0        0        0     1029 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/nvidia.py
--rw-r--r--   0        0        0     1632 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/openai.py
--rw-r--r--   0        0        0      747 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/embedder/vertexai.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/__init__.py
--rw-r--r--   0        0        0      724 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/base.py
--rw-r--r--   0        0        0      175 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/metrics/__init__.py
--rw-r--r--   0        0        0     3600 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/metrics/answer_relevancy.py
--rw-r--r--   0        0        0     2696 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/metrics/context_relevancy.py
--rw-r--r--   0        0        0     4127 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/evaluation/metrics/groundedness.py
--rw-r--r--   0        0        0     5498 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/factory.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/helpers/__init__.py
--rw-r--r--   0        0        0     2359 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/helpers/callbacks.py
--rw-r--r--   0        0        0     7758 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/helpers/json_serializable.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/__init__.py
--rw-r--r--   0        0        0     1245 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/anthropic.py
--rw-r--r--   0        0        0     1645 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/aws_bedrock.py
--rw-r--r--   0        0        0     1372 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/azure_openai.py
--rw-r--r--   0        0        0    12547 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/base.py
--rw-r--r--   0        0        0     1453 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/cohere.py
--rw-r--r--   0        0        0     2331 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/google.py
--rw-r--r--   0        0        0     2675 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/gpt4all.py
--rw-r--r--   0        0        0     1618 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/groq.py
--rw-r--r--   0        0        0     3664 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/huggingface.py
--rw-r--r--   0        0        0     1564 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/jina.py
--rw-r--r--   0        0        0     1927 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/llama2.py
--rw-r--r--   0        0        0     2031 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/mistralai.py
--rw-r--r--   0        0        0     1920 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/nvidia.py
--rw-r--r--   0        0        0     1356 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/ollama.py
--rw-r--r--   0        0        0     2894 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/openai.py
--rw-r--r--   0        0        0     1474 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/together.py
--rw-r--r--   0        0        0     1716 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/vertex_ai.py
--rw-r--r--   0        0        0     1490 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/llm/vllm.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/__init__.py
--rw-r--r--   0        0        0      246 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/base_loader.py
--rw-r--r--   0        0        0     3739 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/beehiiv.py
--rw-r--r--   0        0        0     1903 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/csv.py
--rw-r--r--   0        0        0     2476 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/directory_loader.py
--rw-r--r--   0        0        0     5432 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/discord.py
--rw-r--r--   0        0        0     3132 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/discourse.py
--rw-r--r--   0        0        0     3437 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/docs_site_loader.py
--rw-r--r--   0        0        0      938 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/docx_file.py
--rw-r--r--   0        0        0     3298 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/dropbox.py
--rw-r--r--   0        0        0    12338 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/github.py
--rw-r--r--   0        0        0     5216 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/gmail.py
--rw-r--r--   0        0        0     1996 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/google_drive.py
--rw-r--r--   0        0        0     2042 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/image.py
--rw-r--r--   0        0        0     3086 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/json.py
--rw-r--r--   0        0        0      731 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/local_qna_pair.py
--rw-r--r--   0        0        0      647 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/local_text.py
--rw-r--r--   0        0        0      701 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/mdx.py
--rw-r--r--   0        0        0     2440 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/mysql.py
--rw-r--r--   0        0        0     4178 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/notion.py
--rw-r--r--   0        0        0     1487 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/openapi.py
--rw-r--r--   0        0        0     1503 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/pdf_file.py
--rw-r--r--   0        0        0     2510 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/postgres.py
--rw-r--r--   0        0        0     1593 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/rss_feed.py
--rw-r--r--   0        0        0     2992 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/sitemap.py
--rw-r--r--   0        0        0     3976 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/slack.py
--rw-r--r--   0        0        0     3743 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/substack.py
--rw-r--r--   0        0        0      901 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/text_file.py
--rw-r--r--   0        0        0     1425 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/unstructured_file.py
--rw-r--r--   0        0        0     2986 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/web_page.py
--rw-r--r--   0        0        0     1061 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/xml.py
--rw-r--r--   0        0        0     3071 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/youtube_channel.py
--rw-r--r--   0        0        0     1222 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/loaders/youtube_video.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/memory/__init__.py
--rw-r--r--   0        0        0     4915 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/memory/base.py
--rw-r--r--   0        0        0     2140 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/memory/message.py
--rw-r--r--   0        0        0     1135 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/memory/utils.py
--rw-r--r--   0        0        0     1854 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/migrations/env.py
--rw-r--r--   0        0        0      635 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/migrations/script.py.mako
--rw-r--r--   0        0        0     2672 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/migrations/versions/40a327b3debd_create_initial_migrations.py
--rw-r--r--   0        0        0      175 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/models/__init__.py
--rw-r--r--   0        0        0     2432 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/models/data_type.py
--rw-r--r--   0        0        0      164 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/models/embedding_functions.py
--rw-r--r--   0        0        0      207 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/models/providers.py
--rw-r--r--   0        0        0      266 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/models/vector_dimensions.py
--rw-r--r--   0        0        0      123 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/store/__init__.py
--rw-r--r--   0        0        0     7815 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/store/assistants.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.653444 embedchain-0.1.98/embedchain/telemetry/__init__.py
--rw-r--r--   0        0        0     1961 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/telemetry/posthog.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/utils/__init__.py
--rw-r--r--   0        0        0    12653 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/utils/cli.py
--rw-r--r--   0        0        0      376 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/utils/evaluation.py
--rw-r--r--   0        0        0    19445 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/utils/misc.py
--rw-r--r--   0        0        0        0 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/__init__.py
--rw-r--r--   0        0        0     2463 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/base.py
--rw-r--r--   0        0        0    10792 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/chroma.py
--rw-r--r--   0        0        0    10594 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/elasticsearch.py
--rw-r--r--   0        0        0     9521 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/opensearch.py
--rw-r--r--   0        0        0     9339 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/pinecone.py
--rw-r--r--   0        0        0     9267 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/qdrant.py
--rw-r--r--   0        0        0    14289 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/weaviate.py
--rw-r--r--   0        0        0     8700 2024-03-21 02:30:45.657444 embedchain-0.1.98/embedchain/vectordb/zilliz.py
--rw-r--r--   0        0        0     6298 2024-03-21 02:30:45.665444 embedchain-0.1.98/pyproject.toml
--rw-r--r--   0        0        0    10711 1970-01-01 00:00:00.000000 embedchain-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-20 04:37:16.311453 embedchain-0.1.99/LICENSE
+-rw-r--r--   0        0        0     5650 2024-03-11 17:20:19.838495 embedchain-0.1.99/README.md
+-rw-r--r--   0        0        0      313 2024-02-19 23:47:56.239992 embedchain-0.1.99/embedchain/__init__.py
+-rw-r--r--   0        0        0     3615 2024-03-18 17:35:30.747425 embedchain-0.1.99/embedchain/alembic.ini
+-rw-r--r--   0        0        0    20753 2024-03-28 07:30:01.987810 embedchain-0.1.99/embedchain/app.py
+-rw-r--r--   0        0        0      193 2023-09-09 19:45:33.183212 embedchain-0.1.99/embedchain/bots/__init__.py
+-rw-r--r--   0        0        0     1636 2024-03-14 07:42:54.048825 embedchain-0.1.99/embedchain/bots/base.py
+-rw-r--r--   0        0        0     4335 2024-03-14 07:01:49.927192 embedchain-0.1.99/embedchain/bots/discord.py
+-rw-r--r--   0        0        0     3010 2024-01-09 17:54:02.750902 embedchain-0.1.99/embedchain/bots/poe.py
+-rw-r--r--   0        0        0     3938 2024-03-14 07:01:49.927441 embedchain-0.1.99/embedchain/bots/slack.py
+-rw-r--r--   0        0        0     2689 2024-03-14 07:01:49.927688 embedchain-0.1.99/embedchain/bots/whatsapp.py
+-rw-r--r--   0        0        0     1548 2024-03-14 07:42:54.032425 embedchain-0.1.99/embedchain/cache.py
+-rw-r--r--   0        0        0        0 2023-07-20 04:37:16.317114 embedchain-0.1.99/embedchain/chunkers/__init__.py
+-rw-r--r--   0        0        0     3326 2024-03-14 07:01:49.928213 embedchain-0.1.99/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0        0        0      805 2023-12-14 11:56:34.819095 embedchain-0.1.99/embedchain/chunkers/beehiiv.py
+-rw-r--r--   0        0        0      815 2023-12-14 11:56:34.748421 embedchain-0.1.99/embedchain/chunkers/common_chunker.py
+-rw-r--r--   0        0        0      809 2023-11-23 08:36:44.574725 embedchain-0.1.99/embedchain/chunkers/discourse.py
+-rw-r--r--   0        0        0      813 2023-12-13 07:20:27.387649 embedchain-0.1.99/embedchain/chunkers/docs_site.py
+-rw-r--r--   0        0        0      809 2023-11-23 08:36:44.575018 embedchain-0.1.99/embedchain/chunkers/docx_file.py
+-rw-r--r--   0        0        0      801 2023-11-23 08:36:44.575161 embedchain-0.1.99/embedchain/chunkers/gmail.py
+-rw-r--r--   0        0        0      821 2024-01-05 07:43:18.406969 embedchain-0.1.99/embedchain/chunkers/google_drive.py
+-rw-r--r--   0        0        0      802 2024-01-02 12:09:27.593364 embedchain-0.1.99/embedchain/chunkers/image.py
+-rw-r--r--   0        0        0      799 2023-11-23 08:36:44.575300 embedchain-0.1.99/embedchain/chunkers/json.py
+-rw-r--r--   0        0        0      803 2023-11-23 08:36:44.575451 embedchain-0.1.99/embedchain/chunkers/mdx.py
+-rw-r--r--   0        0        0      800 2023-11-23 08:36:44.575622 embedchain-0.1.99/embedchain/chunkers/mysql.py
+-rw-r--r--   0        0        0      802 2023-11-23 08:36:44.575923 embedchain-0.1.99/embedchain/chunkers/notion.py
+-rw-r--r--   0        0        0      675 2023-10-26 05:43:55.226529 embedchain-0.1.99/embedchain/chunkers/openapi.py
+-rw-r--r--   0        0        0      806 2023-11-23 08:36:44.576274 embedchain-0.1.99/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0        0        0      807 2023-11-23 08:36:44.576551 embedchain-0.1.99/embedchain/chunkers/postgres.py
+-rw-r--r--   0        0        0      805 2023-11-23 08:36:44.576765 embedchain-0.1.99/embedchain/chunkers/qna_pair.py
+-rw-r--r--   0        0        0      806 2024-01-02 12:09:27.594125 embedchain-0.1.99/embedchain/chunkers/rss_feed.py
+-rw-r--r--   0        0        0      804 2023-11-23 08:36:44.576922 embedchain-0.1.99/embedchain/chunkers/sitemap.py
+-rw-r--r--   0        0        0      804 2023-11-23 08:36:44.577092 embedchain-0.1.99/embedchain/chunkers/slack.py
+-rw-r--r--   0        0        0      807 2023-11-23 08:36:44.577240 embedchain-0.1.99/embedchain/chunkers/substack.py
+-rw-r--r--   0        0        0      749 2023-10-06 18:44:00.508600 embedchain-0.1.99/embedchain/chunkers/table.py
+-rw-r--r--   0        0        0      798 2023-11-23 08:36:44.577391 embedchain-0.1.99/embedchain/chunkers/text.py
+-rw-r--r--   0        0        0      824 2023-11-23 08:36:44.577548 embedchain-0.1.99/embedchain/chunkers/unstructured_file.py
+-rw-r--r--   0        0        0      806 2023-12-14 11:56:47.845876 embedchain-0.1.99/embedchain/chunkers/web_page.py
+-rw-r--r--   0        0        0      803 2023-11-23 08:36:44.577855 embedchain-0.1.99/embedchain/chunkers/xml.py
+-rw-r--r--   0        0        0      816 2023-11-23 08:36:44.578041 embedchain-0.1.99/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0        0        0    12794 2024-03-14 07:42:54.037751 embedchain-0.1.99/embedchain/cli.py
+-rw-r--r--   0        0        0     3275 2024-03-14 07:01:49.928478 embedchain-0.1.99/embedchain/client.py
+-rw-r--r--   0        0        0      523 2023-12-30 09:50:00.949563 embedchain-0.1.99/embedchain/config/__init__.py
+-rw-r--r--   0        0        0     2407 2024-01-09 17:54:02.752936 embedchain-0.1.99/embedchain/config/add_config.py
+-rw-r--r--   0        0        0     1282 2023-12-29 11:29:34.606684 embedchain-0.1.99/embedchain/config/app_config.py
+-rw-r--r--   0        0        0     2358 2024-03-14 07:01:49.928722 embedchain-0.1.99/embedchain/config/base_app_config.py
+-rw-r--r--   0        0        0      453 2024-01-09 17:54:02.753204 embedchain-0.1.99/embedchain/config/base_config.py
+-rw-r--r--   0        0        0     3780 2024-01-09 17:54:02.753365 embedchain-0.1.99/embedchain/config/cache_config.py
+-rw-r--r--   0        0        0        0 2023-09-09 19:45:33.187929 embedchain-0.1.99/embedchain/config/embedder/__init__.py
+-rw-r--r--   0        0        0      982 2024-03-05 02:17:55.535271 embedchain-0.1.99/embedchain/config/embedder/base.py
+-rw-r--r--   0        0        0      609 2023-12-19 12:31:23.288385 embedchain-0.1.99/embedchain/config/embedder/google.py
+-rw-r--r--   0        0        0      119 2024-03-14 07:42:54.124198 embedchain-0.1.99/embedchain/config/evaluation/__init__.py
+-rw-r--r--   0        0        0     3457 2024-01-14 06:33:14.895724 embedchain-0.1.99/embedchain/config/evaluation/base.py
+-rw-r--r--   0        0        0        0 2023-09-09 19:45:33.188174 embedchain-0.1.99/embedchain/config/llm/__init__.py
+-rw-r--r--   0        0        0     8336 2024-03-14 07:01:49.929196 embedchain-0.1.99/embedchain/config/llm/base.py
+-rw-r--r--   0        0        0        0 2023-10-06 18:44:00.510984 embedchain-0.1.99/embedchain/config/vectordb/__init__.py
+-rw-r--r--   0        0        0     1385 2023-10-13 08:33:09.754258 embedchain-0.1.99/embedchain/config/vectordb/base.py
+-rw-r--r--   0        0        0     1591 2023-11-23 08:36:44.579573 embedchain-0.1.99/embedchain/config/vectordb/chroma.py
+-rw-r--r--   0        0        0     2438 2024-01-09 17:54:02.754716 embedchain-0.1.99/embedchain/config/vectordb/elasticsearch.py
+-rw-r--r--   0        0        0     1556 2024-01-09 17:54:02.754879 embedchain-0.1.99/embedchain/config/vectordb/opensearch.py
+-rw-r--r--   0        0        0     1859 2024-02-27 19:04:55.805622 embedchain-0.1.99/embedchain/config/vectordb/pinecone.py
+-rw-r--r--   0        0        0     1993 2024-01-09 17:54:02.755371 embedchain-0.1.99/embedchain/config/vectordb/qdrant.py
+-rw-r--r--   0        0        0      505 2024-01-09 17:54:02.755619 embedchain-0.1.99/embedchain/config/vectordb/weaviate.py
+-rw-r--r--   0        0        0     2055 2024-01-08 20:41:12.610668 embedchain-0.1.99/embedchain/config/vectordb/zilliz.py
+-rw-r--r--   0        0        0      372 2024-02-22 07:14:32.810472 embedchain-0.1.99/embedchain/constants.py
+-rw-r--r--   0        0        0        0 2024-02-19 23:47:56.241106 embedchain-0.1.99/embedchain/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-19 23:47:56.241326 embedchain-0.1.99/embedchain/core/db/__init__.py
+-rw-r--r--   0        0        0     3043 2024-03-14 07:39:59.280495 embedchain-0.1.99/embedchain/core/db/database.py
+-rw-r--r--   0        0        0      944 2024-02-19 23:47:56.241721 embedchain-0.1.99/embedchain/core/db/models.py
+-rw-r--r--   0        0        0       56 2023-10-28 04:33:01.398059 embedchain-0.1.99/embedchain/data_formatter/__init__.py
+-rw-r--r--   0        0        0     7743 2024-01-08 20:41:12.611245 embedchain-0.1.99/embedchain/data_formatter/data_formatter.py
+-rw-r--r--   0        0        0        3 2023-12-19 12:31:23.298911 embedchain-0.1.99/embedchain/deployment/fly.io/.dockerignore
+-rw-r--r--   0        0        0       21 2023-12-19 12:31:23.299422 embedchain-0.1.99/embedchain/deployment/fly.io/.env.example
+-rw-r--r--   0        0        0      195 2023-12-19 12:31:23.299712 embedchain-0.1.99/embedchain/deployment/fly.io/Dockerfile
+-rw-r--r--   0        0        0     1296 2024-02-12 00:47:28.550526 embedchain-0.1.99/embedchain/deployment/fly.io/app.py
+-rw-r--r--   0        0        0       58 2023-12-20 04:26:04.091267 embedchain-0.1.99/embedchain/deployment/fly.io/requirements.txt
+-rw-r--r--   0        0        0      221 2023-12-29 11:29:34.606860 embedchain-0.1.99/embedchain/deployment/gradio.app/app.py
+-rw-r--r--   0        0        0       26 2023-12-22 13:26:07.493929 embedchain-0.1.99/embedchain/deployment/gradio.app/requirements.txt
+-rw-r--r--   0        0        0       21 2023-12-22 13:26:07.494289 embedchain-0.1.99/embedchain/deployment/modal.com/.env.example
+-rw-r--r--   0        0        0        5 2023-12-19 12:31:23.300510 embedchain-0.1.99/embedchain/deployment/modal.com/.gitignore
+-rw-r--r--   0        0        0     1913 2024-02-12 00:47:28.550978 embedchain-0.1.99/embedchain/deployment/modal.com/app.py
+-rw-r--r--   0        0        0       61 2023-12-20 04:26:04.091475 embedchain-0.1.99/embedchain/deployment/modal.com/requirements.txt
+-rw-r--r--   0        0        0       21 2023-12-21 08:56:07.352537 embedchain-0.1.99/embedchain/deployment/render.com/.env.example
+-rw-r--r--   0        0        0        5 2023-12-21 08:56:07.352863 embedchain-0.1.99/embedchain/deployment/render.com/.gitignore
+-rw-r--r--   0        0        0     1244 2024-02-12 00:47:28.551349 embedchain-0.1.99/embedchain/deployment/render.com/app.py
+-rw-r--r--   0        0        0      506 2023-12-21 08:56:07.353470 embedchain-0.1.99/embedchain/deployment/render.com/render.yaml
+-rw-r--r--   0        0        0       58 2023-12-21 08:56:07.353713 embedchain-0.1.99/embedchain/deployment/render.com/requirements.txt
+-rw-r--r--   0        0        0       24 2023-12-21 08:56:07.353911 embedchain-0.1.99/embedchain/deployment/streamlit.io/.streamlit/secrets.toml
+-rw-r--r--   0        0        0     1962 2023-12-29 11:29:34.606982 embedchain-0.1.99/embedchain/deployment/streamlit.io/app.py
+-rw-r--r--   0        0        0       29 2023-12-21 08:56:07.354271 embedchain-0.1.99/embedchain/deployment/streamlit.io/requirements.txt
+-rw-r--r--   0        0        0    29680 2024-03-14 07:42:54.028081 embedchain-0.1.99/embedchain/embedchain.py
+-rw-r--r--   0        0        0        0 2023-09-09 19:45:33.189069 embedchain-0.1.99/embedchain/embedder/__init__.py
+-rw-r--r--   0        0        0     3001 2024-01-10 07:10:23.419226 embedchain-0.1.99/embedchain/embedder/base.py
+-rw-r--r--   0        0        0      738 2024-03-14 00:01:37.647250 embedchain-0.1.99/embedchain/embedder/cohere.py
+-rw-r--r--   0        0        0     1459 2024-01-29 12:57:52.348219 embedchain-0.1.99/embedchain/embedder/google.py
+-rw-r--r--   0        0        0      770 2024-03-14 07:42:54.181784 embedchain-0.1.99/embedchain/embedder/gpt4all.py
+-rw-r--r--   0        0        0      764 2024-02-13 01:22:09.959177 embedchain-0.1.99/embedchain/embedder/huggingface.py
+-rw-r--r--   0        0        0     1711 2024-01-29 12:57:52.349137 embedchain-0.1.99/embedchain/embedder/mistralai.py
+-rw-r--r--   0        0        0     1029 2024-03-14 07:01:49.930022 embedchain-0.1.99/embedchain/embedder/nvidia.py
+-rw-r--r--   0        0        0     1632 2024-03-06 00:04:24.307982 embedchain-0.1.99/embedchain/embedder/openai.py
+-rw-r--r--   0        0        0      747 2024-02-13 01:22:09.959647 embedchain-0.1.99/embedchain/embedder/vertexai.py
+-rw-r--r--   0        0        0        0 2024-01-14 06:33:14.895767 embedchain-0.1.99/embedchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      724 2024-01-14 06:33:14.896055 embedchain-0.1.99/embedchain/evaluation/base.py
+-rw-r--r--   0        0        0      175 2024-01-14 06:33:14.896150 embedchain-0.1.99/embedchain/evaluation/metrics/__init__.py
+-rw-r--r--   0        0        0     3600 2024-03-14 07:01:49.930311 embedchain-0.1.99/embedchain/evaluation/metrics/answer_relevancy.py
+-rw-r--r--   0        0        0     2696 2024-01-14 06:33:14.896671 embedchain-0.1.99/embedchain/evaluation/metrics/context_relevancy.py
+-rw-r--r--   0        0        0     4127 2024-03-14 07:01:49.930556 embedchain-0.1.99/embedchain/evaluation/metrics/groundedness.py
+-rw-r--r--   0        0        0     5498 2024-03-14 07:01:49.930807 embedchain-0.1.99/embedchain/factory.py
+-rw-r--r--   0        0        0        0 2023-11-23 08:36:44.581372 embedchain-0.1.99/embedchain/helpers/__init__.py
+-rw-r--r--   0        0        0     2359 2024-02-27 23:11:12.536725 embedchain-0.1.99/embedchain/helpers/callbacks.py
+-rw-r--r--   0        0        0     7758 2024-03-14 07:01:49.931265 embedchain-0.1.99/embedchain/helpers/json_serializable.py
+-rw-r--r--   0        0        0        0 2023-09-09 19:45:33.189723 embedchain-0.1.99/embedchain/llm/__init__.py
+-rw-r--r--   0        0        0     1378 2024-03-28 08:21:17.927686 embedchain-0.1.99/embedchain/llm/anthropic.py
+-rw-r--r--   0        0        0     1645 2024-03-14 07:42:54.064100 embedchain-0.1.99/embedchain/llm/aws_bedrock.py
+-rw-r--r--   0        0        0     1372 2024-03-14 07:01:49.932040 embedchain-0.1.99/embedchain/llm/azure_openai.py
+-rw-r--r--   0        0        0    12547 2024-03-14 07:42:54.079266 embedchain-0.1.99/embedchain/llm/base.py
+-rw-r--r--   0        0        0     1453 2024-02-27 23:11:12.537309 embedchain-0.1.99/embedchain/llm/cohere.py
+-rw-r--r--   0        0        0     2331 2024-03-14 07:01:49.932440 embedchain-0.1.99/embedchain/llm/google.py
+-rw-r--r--   0        0        0     2675 2024-03-14 07:42:54.063053 embedchain-0.1.99/embedchain/llm/gpt4all.py
+-rw-r--r--   0        0        0     1618 2024-02-25 23:12:48.081378 embedchain-0.1.99/embedchain/llm/groq.py
+-rw-r--r--   0        0        0     3664 2024-03-14 07:01:49.932628 embedchain-0.1.99/embedchain/llm/huggingface.py
+-rw-r--r--   0        0        0     1564 2024-03-14 07:42:54.060201 embedchain-0.1.99/embedchain/llm/jina.py
+-rw-r--r--   0        0        0     1927 2024-02-27 23:11:12.537489 embedchain-0.1.99/embedchain/llm/llama2.py
+-rw-r--r--   0        0        0     2031 2024-01-29 12:57:52.350685 embedchain-0.1.99/embedchain/llm/mistralai.py
+-rw-r--r--   0        0        0     1920 2024-03-01 19:43:20.607038 embedchain-0.1.99/embedchain/llm/nvidia.py
+-rw-r--r--   0        0        0     1356 2024-03-05 02:17:55.536833 embedchain-0.1.99/embedchain/llm/ollama.py
+-rw-r--r--   0        0        0     2894 2024-03-14 07:42:54.067692 embedchain-0.1.99/embedchain/llm/openai.py
+-rw-r--r--   0        0        0     1474 2024-02-27 23:11:12.537935 embedchain-0.1.99/embedchain/llm/together.py
+-rw-r--r--   0        0        0     1716 2024-03-14 07:01:49.933075 embedchain-0.1.99/embedchain/llm/vertex_ai.py
+-rw-r--r--   0        0        0     1490 2024-02-27 23:11:12.538245 embedchain-0.1.99/embedchain/llm/vllm.py
+-rw-r--r--   0        0        0        0 2023-07-20 04:37:16.318903 embedchain-0.1.99/embedchain/loaders/__init__.py
+-rw-r--r--   0        0        0      246 2024-01-08 20:41:12.615584 embedchain-0.1.99/embedchain/loaders/base_loader.py
+-rw-r--r--   0        0        0     3739 2024-03-14 07:01:49.933264 embedchain-0.1.99/embedchain/loaders/beehiiv.py
+-rw-r--r--   0        0        0     1903 2023-09-27 20:28:42.457626 embedchain-0.1.99/embedchain/loaders/csv.py
+-rw-r--r--   0        0        0     2476 2024-03-14 07:01:49.933546 embedchain-0.1.99/embedchain/loaders/directory_loader.py
+-rw-r--r--   0        0        0     5432 2024-03-14 07:01:49.933741 embedchain-0.1.99/embedchain/loaders/discord.py
+-rw-r--r--   0        0        0     3132 2024-03-14 07:01:49.933918 embedchain-0.1.99/embedchain/loaders/discourse.py
+-rw-r--r--   0        0        0     3437 2024-03-14 07:01:49.934102 embedchain-0.1.99/embedchain/loaders/docs_site_loader.py
+-rw-r--r--   0        0        0      938 2024-02-18 22:33:47.577036 embedchain-0.1.99/embedchain/loaders/docx_file.py
+-rw-r--r--   0        0        0     3298 2024-01-09 17:54:02.761249 embedchain-0.1.99/embedchain/loaders/dropbox.py
+-rw-r--r--   0        0        0    12338 2024-03-14 00:02:09.704548 embedchain-0.1.99/embedchain/loaders/github.py
+-rw-r--r--   0        0        0     5216 2024-03-14 07:01:49.934423 embedchain-0.1.99/embedchain/loaders/gmail.py
+-rw-r--r--   0        0        0     1996 2024-02-13 01:22:09.962587 embedchain-0.1.99/embedchain/loaders/google_drive.py
+-rw-r--r--   0        0        0     2042 2024-01-08 20:41:12.616324 embedchain-0.1.99/embedchain/loaders/image.py
+-rw-r--r--   0        0        0     3086 2024-02-12 00:47:28.560295 embedchain-0.1.99/embedchain/loaders/json.py
+-rw-r--r--   0        0        0      731 2024-02-18 22:33:47.577200 embedchain-0.1.99/embedchain/loaders/local_qna_pair.py
+-rw-r--r--   0        0        0      647 2024-02-18 22:33:47.577352 embedchain-0.1.99/embedchain/loaders/local_text.py
+-rw-r--r--   0        0        0      701 2024-02-18 22:33:47.577526 embedchain-0.1.99/embedchain/loaders/mdx.py
+-rw-r--r--   0        0        0     2440 2024-03-14 07:01:49.934605 embedchain-0.1.99/embedchain/loaders/mysql.py
+-rw-r--r--   0        0        0     4178 2024-03-14 07:01:49.934921 embedchain-0.1.99/embedchain/loaders/notion.py
+-rw-r--r--   0        0        0     1487 2024-02-18 22:33:47.577678 embedchain-0.1.99/embedchain/loaders/openapi.py
+-rw-r--r--   0        0        0     1503 2024-02-18 22:33:47.577952 embedchain-0.1.99/embedchain/loaders/pdf_file.py
+-rw-r--r--   0        0        0     2510 2024-03-14 07:01:49.935171 embedchain-0.1.99/embedchain/loaders/postgres.py
+-rw-r--r--   0        0        0     1593 2024-03-14 07:42:54.258007 embedchain-0.1.99/embedchain/loaders/rss_feed.py
+-rw-r--r--   0        0        0     2992 2024-03-14 07:01:49.935374 embedchain-0.1.99/embedchain/loaders/sitemap.py
+-rw-r--r--   0        0        0     3976 2024-03-14 07:01:49.935644 embedchain-0.1.99/embedchain/loaders/slack.py
+-rw-r--r--   0        0        0     3743 2024-03-14 07:01:49.935840 embedchain-0.1.99/embedchain/loaders/substack.py
+-rw-r--r--   0        0        0      901 2024-02-18 22:33:47.578439 embedchain-0.1.99/embedchain/loaders/text_file.py
+-rw-r--r--   0        0        0     1425 2024-03-14 07:42:54.259785 embedchain-0.1.99/embedchain/loaders/unstructured_file.py
+-rw-r--r--   0        0        0     2986 2024-03-14 07:01:49.936042 embedchain-0.1.99/embedchain/loaders/web_page.py
+-rw-r--r--   0        0        0     1061 2024-02-18 22:33:47.579043 embedchain-0.1.99/embedchain/loaders/xml.py
+-rw-r--r--   0        0        0     3071 2024-03-14 07:01:49.936231 embedchain-0.1.99/embedchain/loaders/youtube_channel.py
+-rw-r--r--   0        0        0     1222 2024-02-18 22:33:47.579353 embedchain-0.1.99/embedchain/loaders/youtube_video.py
+-rw-r--r--   0        0        0        0 2023-11-09 21:57:56.964406 embedchain-0.1.99/embedchain/memory/__init__.py
+-rw-r--r--   0        0        0     4915 2024-03-14 07:01:49.936425 embedchain-0.1.99/embedchain/memory/base.py
+-rw-r--r--   0        0        0     2140 2024-03-14 07:01:49.936609 embedchain-0.1.99/embedchain/memory/message.py
+-rw-r--r--   0        0        0     1135 2024-01-09 17:54:02.765110 embedchain-0.1.99/embedchain/memory/utils.py
+-rw-r--r--   0        0        0     1854 2024-03-18 17:35:30.748129 embedchain-0.1.99/embedchain/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-02-19 23:47:56.242554 embedchain-0.1.99/embedchain/migrations/script.py.mako
+-rw-r--r--   0        0        0     2672 2024-02-19 23:47:56.242702 embedchain-0.1.99/embedchain/migrations/versions/40a327b3debd_create_initial_migrations.py
+-rw-r--r--   0        0        0      175 2023-11-10 00:53:36.738741 embedchain-0.1.99/embedchain/models/__init__.py
+-rw-r--r--   0        0        0     2432 2024-01-05 07:43:18.408300 embedchain-0.1.99/embedchain/models/data_type.py
+-rw-r--r--   0        0        0      164 2023-10-06 20:43:54.836892 embedchain-0.1.99/embedchain/models/embedding_functions.py
+-rw-r--r--   0        0        0      207 2023-12-22 13:26:07.495803 embedchain-0.1.99/embedchain/models/providers.py
+-rw-r--r--   0        0        0      266 2024-03-14 00:01:37.653510 embedchain-0.1.99/embedchain/models/vector_dimensions.py
+-rw-r--r--   0        0        0      123 2023-12-29 18:45:29.207064 embedchain-0.1.99/embedchain/pipeline.py
+-rw-r--r--   0        0        0        0 2023-11-09 07:32:59.306048 embedchain-0.1.99/embedchain/store/__init__.py
+-rw-r--r--   0        0        0     7815 2024-03-14 07:01:49.936905 embedchain-0.1.99/embedchain/store/assistants.py
+-rw-r--r--   0        0        0        0 2023-10-29 21:47:26.730972 embedchain-0.1.99/embedchain/telemetry/__init__.py
+-rw-r--r--   0        0        0     1961 2024-03-01 19:43:20.607987 embedchain-0.1.99/embedchain/telemetry/posthog.py
+-rw-r--r--   0        0        0        0 2024-01-05 15:01:47.809672 embedchain-0.1.99/embedchain/utils/__init__.py
+-rw-r--r--   0        0        0    12653 2024-01-05 15:01:47.810176 embedchain-0.1.99/embedchain/utils/cli.py
+-rw-r--r--   0        0        0      376 2024-01-14 06:33:14.896997 embedchain-0.1.99/embedchain/utils/evaluation.py
+-rw-r--r--   0        0        0    19445 2024-03-28 07:23:55.271499 embedchain-0.1.99/embedchain/utils/misc.py
+-rw-r--r--   0        0        0        0 2023-07-20 04:37:16.319825 embedchain-0.1.99/embedchain/vectordb/__init__.py
+-rw-r--r--   0        0        0     2463 2024-01-29 12:57:52.353186 embedchain-0.1.99/embedchain/vectordb/base.py
+-rw-r--r--   0        0        0    10792 2024-03-14 07:01:49.937500 embedchain-0.1.99/embedchain/vectordb/chroma.py
+-rw-r--r--   0        0        0    10594 2024-03-14 07:01:49.937753 embedchain-0.1.99/embedchain/vectordb/elasticsearch.py
+-rw-r--r--   0        0        0     9521 2024-03-14 07:01:49.938135 embedchain-0.1.99/embedchain/vectordb/opensearch.py
+-rw-r--r--   0        0        0     9339 2024-03-26 23:17:56.713975 embedchain-0.1.99/embedchain/vectordb/pinecone.py
+-rw-r--r--   0        0        0     9255 2024-03-28 08:21:17.928012 embedchain-0.1.99/embedchain/vectordb/qdrant.py
+-rw-r--r--   0        0        0    14289 2024-02-12 00:47:28.563951 embedchain-0.1.99/embedchain/vectordb/weaviate.py
+-rw-r--r--   0        0        0     8700 2024-03-14 07:42:54.168776 embedchain-0.1.99/embedchain/vectordb/zilliz.py
+-rw-r--r--   0        0        0     6299 2024-03-28 08:21:17.928627 embedchain-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0    10661 1970-01-01 00:00:00.000000 embedchain-0.1.99/PKG-INFO
```

### Comparing `embedchain-0.1.98/LICENSE` & `embedchain-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/README.md` & `embedchain-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/alembic.ini` & `embedchain-0.1.99/embedchain/alembic.ini`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/app.py` & `embedchain-0.1.99/embedchain/app.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/bots/base.py` & `embedchain-0.1.99/embedchain/bots/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/bots/discord.py` & `embedchain-0.1.99/embedchain/bots/discord.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/bots/poe.py` & `embedchain-0.1.99/embedchain/bots/poe.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/bots/slack.py` & `embedchain-0.1.99/embedchain/bots/slack.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/bots/whatsapp.py` & `embedchain-0.1.99/embedchain/bots/whatsapp.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/cache.py` & `embedchain-0.1.99/embedchain/cache.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/base_chunker.py` & `embedchain-0.1.99/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/beehiiv.py` & `embedchain-0.1.99/embedchain/chunkers/beehiiv.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/common_chunker.py` & `embedchain-0.1.99/embedchain/chunkers/common_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/discourse.py` & `embedchain-0.1.99/embedchain/chunkers/discourse.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/docs_site.py` & `embedchain-0.1.99/embedchain/chunkers/docs_site.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/docx_file.py` & `embedchain-0.1.99/embedchain/chunkers/docx_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/gmail.py` & `embedchain-0.1.99/embedchain/chunkers/gmail.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/google_drive.py` & `embedchain-0.1.99/embedchain/chunkers/google_drive.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/image.py` & `embedchain-0.1.99/embedchain/chunkers/image.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/json.py` & `embedchain-0.1.99/embedchain/chunkers/json.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/mdx.py` & `embedchain-0.1.99/embedchain/chunkers/mdx.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/mysql.py` & `embedchain-0.1.99/embedchain/chunkers/mysql.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/notion.py` & `embedchain-0.1.99/embedchain/chunkers/notion.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/openapi.py` & `embedchain-0.1.99/embedchain/chunkers/openapi.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/pdf_file.py` & `embedchain-0.1.99/embedchain/chunkers/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/postgres.py` & `embedchain-0.1.99/embedchain/chunkers/postgres.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/qna_pair.py` & `embedchain-0.1.99/embedchain/chunkers/qna_pair.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/rss_feed.py` & `embedchain-0.1.99/embedchain/chunkers/rss_feed.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/sitemap.py` & `embedchain-0.1.99/embedchain/chunkers/sitemap.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/slack.py` & `embedchain-0.1.99/embedchain/chunkers/slack.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/substack.py` & `embedchain-0.1.99/embedchain/chunkers/substack.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/table.py` & `embedchain-0.1.99/embedchain/chunkers/table.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/text.py` & `embedchain-0.1.99/embedchain/chunkers/text.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/unstructured_file.py` & `embedchain-0.1.99/embedchain/chunkers/unstructured_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/web_page.py` & `embedchain-0.1.99/embedchain/chunkers/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/xml.py` & `embedchain-0.1.99/embedchain/chunkers/xml.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/chunkers/youtube_video.py` & `embedchain-0.1.99/embedchain/chunkers/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/cli.py` & `embedchain-0.1.99/embedchain/cli.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/client.py` & `embedchain-0.1.99/embedchain/client.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/__init__.py` & `embedchain-0.1.99/embedchain/config/__init__.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/add_config.py` & `embedchain-0.1.99/embedchain/config/add_config.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/app_config.py` & `embedchain-0.1.99/embedchain/config/app_config.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/base_app_config.py` & `embedchain-0.1.99/embedchain/config/base_app_config.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/cache_config.py` & `embedchain-0.1.99/embedchain/config/cache_config.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/embedder/base.py` & `embedchain-0.1.99/embedchain/config/embedder/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/embedder/google.py` & `embedchain-0.1.99/embedchain/config/embedder/google.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/evaluation/base.py` & `embedchain-0.1.99/embedchain/config/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/llm/base.py` & `embedchain-0.1.99/embedchain/config/llm/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/base.py` & `embedchain-0.1.99/embedchain/config/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/chroma.py` & `embedchain-0.1.99/embedchain/config/vectordb/chroma.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/elasticsearch.py` & `embedchain-0.1.99/embedchain/config/vectordb/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/opensearch.py` & `embedchain-0.1.99/embedchain/config/vectordb/opensearch.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/pinecone.py` & `embedchain-0.1.99/embedchain/config/vectordb/pinecone.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/qdrant.py` & `embedchain-0.1.99/embedchain/config/vectordb/qdrant.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/config/vectordb/zilliz.py` & `embedchain-0.1.99/embedchain/config/vectordb/zilliz.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/core/db/database.py` & `embedchain-0.1.99/embedchain/core/db/database.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/core/db/models.py` & `embedchain-0.1.99/embedchain/core/db/models.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/data_formatter/data_formatter.py` & `embedchain-0.1.99/embedchain/data_formatter/data_formatter.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/deployment/fly.io/app.py` & `embedchain-0.1.99/embedchain/deployment/fly.io/app.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/deployment/modal.com/app.py` & `embedchain-0.1.99/embedchain/deployment/modal.com/app.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/deployment/render.com/app.py` & `embedchain-0.1.99/embedchain/deployment/render.com/app.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/deployment/streamlit.io/app.py` & `embedchain-0.1.99/embedchain/deployment/streamlit.io/app.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedchain.py` & `embedchain-0.1.99/embedchain/embedchain.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/base.py` & `embedchain-0.1.99/embedchain/embedder/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/cohere.py` & `embedchain-0.1.99/embedchain/embedder/cohere.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/google.py` & `embedchain-0.1.99/embedchain/embedder/google.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/gpt4all.py` & `embedchain-0.1.99/embedchain/embedder/gpt4all.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/huggingface.py` & `embedchain-0.1.99/embedchain/embedder/huggingface.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/mistralai.py` & `embedchain-0.1.99/embedchain/embedder/mistralai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/nvidia.py` & `embedchain-0.1.99/embedchain/embedder/nvidia.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/openai.py` & `embedchain-0.1.99/embedchain/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/embedder/vertexai.py` & `embedchain-0.1.99/embedchain/embedder/vertexai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/evaluation/base.py` & `embedchain-0.1.99/embedchain/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/evaluation/metrics/answer_relevancy.py` & `embedchain-0.1.99/embedchain/evaluation/metrics/answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/evaluation/metrics/context_relevancy.py` & `embedchain-0.1.99/embedchain/evaluation/metrics/context_relevancy.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/evaluation/metrics/groundedness.py` & `embedchain-0.1.99/embedchain/evaluation/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/factory.py` & `embedchain-0.1.99/embedchain/factory.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/helpers/callbacks.py` & `embedchain-0.1.99/embedchain/helpers/callbacks.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/helpers/json_serializable.py` & `embedchain-0.1.99/embedchain/helpers/json_serializable.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/anthropic.py` & `embedchain-0.1.99/embedchain/llm/together.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-import logging
+import importlib
 import os
 from typing import Optional
 
+from langchain_community.llms import Together
+
 from embedchain.config import BaseLlmConfig
 from embedchain.helpers.json_serializable import register_deserializable
 from embedchain.llm.base import BaseLlm
 
-logger = logging.getLogger(__name__)
-
 
 @register_deserializable
-class AnthropicLlm(BaseLlm):
+class TogetherLlm(BaseLlm):
     def __init__(self, config: Optional[BaseLlmConfig] = None):
-        if "ANTHROPIC_API_KEY" not in os.environ:
-            raise ValueError("Please set the ANTHROPIC_API_KEY environment variable.")
+        if "TOGETHER_API_KEY" not in os.environ:
+            raise ValueError("Please set the TOGETHER_API_KEY environment variable.")
+
+        try:
+            importlib.import_module("together")
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "The required dependencies for Together are not installed."
+                'Please install with `pip install --upgrade "embedchain[together]"`'
+            ) from None
+
         super().__init__(config=config)
 
     def get_llm_model_answer(self, prompt):
-        return AnthropicLlm._get_answer(prompt=prompt, config=self.config)
+        if self.config.system_prompt:
+            raise ValueError("TogetherLlm does not support `system_prompt`")
+        return TogetherLlm._get_answer(prompt=prompt, config=self.config)
 
     @staticmethod
     def _get_answer(prompt: str, config: BaseLlmConfig) -> str:
-        from langchain_community.chat_models import ChatAnthropic
-
-        chat = ChatAnthropic(
-            anthropic_api_key=os.environ["ANTHROPIC_API_KEY"], temperature=config.temperature, model=config.model
+        llm = Together(
+            together_api_key=os.environ["TOGETHER_API_KEY"],
+            model=config.model,
+            max_tokens=config.max_tokens,
+            temperature=config.temperature,
+            top_p=config.top_p,
         )
 
-        if config.max_tokens and config.max_tokens != 1000:
-            logger.warning("Config option `max_tokens` is not supported by this model.")
-
-        messages = BaseLlm._get_messages(prompt, system_prompt=config.system_prompt)
-
-        return chat(messages).content
+        return llm.invoke(prompt)
```

### Comparing `embedchain-0.1.98/embedchain/llm/aws_bedrock.py` & `embedchain-0.1.99/embedchain/llm/aws_bedrock.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/azure_openai.py` & `embedchain-0.1.99/embedchain/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/base.py` & `embedchain-0.1.99/embedchain/llm/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/cohere.py` & `embedchain-0.1.99/embedchain/llm/cohere.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/google.py` & `embedchain-0.1.99/embedchain/llm/google.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/gpt4all.py` & `embedchain-0.1.99/embedchain/llm/gpt4all.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/groq.py` & `embedchain-0.1.99/embedchain/llm/groq.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/huggingface.py` & `embedchain-0.1.99/embedchain/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/jina.py` & `embedchain-0.1.99/embedchain/llm/jina.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/llama2.py` & `embedchain-0.1.99/embedchain/llm/llama2.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/mistralai.py` & `embedchain-0.1.99/embedchain/llm/mistralai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/nvidia.py` & `embedchain-0.1.99/embedchain/llm/nvidia.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/ollama.py` & `embedchain-0.1.99/embedchain/llm/ollama.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/openai.py` & `embedchain-0.1.99/embedchain/llm/openai.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/llm/together.py` & `embedchain-0.1.99/embedchain/llm/vertex_ai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import importlib
-import os
+import logging
 from typing import Optional
 
-from langchain_community.llms import Together
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
+from langchain_google_vertexai import ChatVertexAI
 
 from embedchain.config import BaseLlmConfig
 from embedchain.helpers.json_serializable import register_deserializable
 from embedchain.llm.base import BaseLlm
 
+logger = logging.getLogger(__name__)
+
 
 @register_deserializable
-class TogetherLlm(BaseLlm):
+class VertexAILlm(BaseLlm):
     def __init__(self, config: Optional[BaseLlmConfig] = None):
-        if "TOGETHER_API_KEY" not in os.environ:
-            raise ValueError("Please set the TOGETHER_API_KEY environment variable.")
-
         try:
-            importlib.import_module("together")
+            importlib.import_module("vertexai")
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
-                "The required dependencies for Together are not installed."
-                'Please install with `pip install --upgrade "embedchain[together]"`'
+                "The required dependencies for VertexAI are not installed."
+                'Please install with `pip install --upgrade "embedchain[vertexai]"`'
             ) from None
-
         super().__init__(config=config)
 
     def get_llm_model_answer(self, prompt):
-        if self.config.system_prompt:
-            raise ValueError("TogetherLlm does not support `system_prompt`")
-        return TogetherLlm._get_answer(prompt=prompt, config=self.config)
+        return VertexAILlm._get_answer(prompt=prompt, config=self.config)
 
     @staticmethod
     def _get_answer(prompt: str, config: BaseLlmConfig) -> str:
-        llm = Together(
-            together_api_key=os.environ["TOGETHER_API_KEY"],
-            model=config.model,
-            max_tokens=config.max_tokens,
-            temperature=config.temperature,
-            top_p=config.top_p,
-        )
+        if config.top_p and config.top_p != 1:
+            logger.warning("Config option `top_p` is not supported by this model.")
+
+        messages = BaseLlm._get_messages(prompt, system_prompt=config.system_prompt)
+
+        if config.stream:
+            callbacks = config.callbacks if config.callbacks else [StreamingStdOutCallbackHandler()]
+            llm = ChatVertexAI(
+                temperature=config.temperature, model=config.model, callbacks=callbacks, streaming=config.stream
+            )
+        else:
+            llm = ChatVertexAI(temperature=config.temperature, model=config.model)
 
-        return llm.invoke(prompt)
+        return llm.invoke(messages).content
```

### Comparing `embedchain-0.1.98/embedchain/llm/vertex_ai.py` & `embedchain-0.1.99/embedchain/llm/vllm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-import importlib
-import logging
-from typing import Optional
+from typing import Iterable, Optional, Union
 
+from langchain.callbacks.manager import CallbackManager
+from langchain.callbacks.stdout import StdOutCallbackHandler
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
-from langchain_google_vertexai import ChatVertexAI
+from langchain_community.llms import VLLM as BaseVLLM
 
 from embedchain.config import BaseLlmConfig
 from embedchain.helpers.json_serializable import register_deserializable
 from embedchain.llm.base import BaseLlm
 
-logger = logging.getLogger(__name__)
-
 
 @register_deserializable
-class VertexAILlm(BaseLlm):
+class VLLM(BaseLlm):
     def __init__(self, config: Optional[BaseLlmConfig] = None):
-        try:
-            importlib.import_module("vertexai")
-        except ModuleNotFoundError:
-            raise ModuleNotFoundError(
-                "The required dependencies for VertexAI are not installed."
-                'Please install with `pip install --upgrade "embedchain[vertexai]"`'
-            ) from None
         super().__init__(config=config)
+        if self.config.model is None:
+            self.config.model = "mosaicml/mpt-7b"
 
     def get_llm_model_answer(self, prompt):
-        return VertexAILlm._get_answer(prompt=prompt, config=self.config)
+        return self._get_answer(prompt=prompt, config=self.config)
 
     @staticmethod
-    def _get_answer(prompt: str, config: BaseLlmConfig) -> str:
-        if config.top_p and config.top_p != 1:
-            logger.warning("Config option `top_p` is not supported by this model.")
-
-        messages = BaseLlm._get_messages(prompt, system_prompt=config.system_prompt)
-
-        if config.stream:
-            callbacks = config.callbacks if config.callbacks else [StreamingStdOutCallbackHandler()]
-            llm = ChatVertexAI(
-                temperature=config.temperature, model=config.model, callbacks=callbacks, streaming=config.stream
-            )
-        else:
-            llm = ChatVertexAI(temperature=config.temperature, model=config.model)
+    def _get_answer(prompt: str, config: BaseLlmConfig) -> Union[str, Iterable]:
+        callback_manager = [StreamingStdOutCallbackHandler()] if config.stream else [StdOutCallbackHandler()]
+
+        # Prepare the arguments for BaseVLLM
+        llm_args = {
+            "model": config.model,
+            "temperature": config.temperature,
+            "top_p": config.top_p,
+            "callback_manager": CallbackManager(callback_manager),
+        }
+
+        # Add model_kwargs if they are not None
+        if config.model_kwargs is not None:
+            llm_args.update(config.model_kwargs)
 
-        return llm.invoke(messages).content
+        llm = BaseVLLM(**llm_args)
+        return llm.invoke(prompt)
```

### Comparing `embedchain-0.1.98/embedchain/loaders/beehiiv.py` & `embedchain-0.1.99/embedchain/loaders/beehiiv.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/csv.py` & `embedchain-0.1.99/embedchain/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/directory_loader.py` & `embedchain-0.1.99/embedchain/loaders/directory_loader.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/discord.py` & `embedchain-0.1.99/embedchain/loaders/discord.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/discourse.py` & `embedchain-0.1.99/embedchain/loaders/discourse.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/docs_site_loader.py` & `embedchain-0.1.99/embedchain/loaders/docs_site_loader.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/docx_file.py` & `embedchain-0.1.99/embedchain/loaders/docx_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/dropbox.py` & `embedchain-0.1.99/embedchain/loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/github.py` & `embedchain-0.1.99/embedchain/loaders/github.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/gmail.py` & `embedchain-0.1.99/embedchain/loaders/gmail.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/google_drive.py` & `embedchain-0.1.99/embedchain/loaders/google_drive.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/image.py` & `embedchain-0.1.99/embedchain/loaders/image.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/json.py` & `embedchain-0.1.99/embedchain/loaders/json.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/local_qna_pair.py` & `embedchain-0.1.99/embedchain/loaders/local_qna_pair.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/local_text.py` & `embedchain-0.1.99/embedchain/loaders/local_text.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/mdx.py` & `embedchain-0.1.99/embedchain/loaders/mdx.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/mysql.py` & `embedchain-0.1.99/embedchain/loaders/mysql.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/notion.py` & `embedchain-0.1.99/embedchain/loaders/notion.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/openapi.py` & `embedchain-0.1.99/embedchain/loaders/openapi.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/pdf_file.py` & `embedchain-0.1.99/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/postgres.py` & `embedchain-0.1.99/embedchain/loaders/postgres.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/rss_feed.py` & `embedchain-0.1.99/embedchain/loaders/rss_feed.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/sitemap.py` & `embedchain-0.1.99/embedchain/loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/slack.py` & `embedchain-0.1.99/embedchain/loaders/slack.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/substack.py` & `embedchain-0.1.99/embedchain/loaders/substack.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/text_file.py` & `embedchain-0.1.99/embedchain/loaders/text_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/unstructured_file.py` & `embedchain-0.1.99/embedchain/loaders/unstructured_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/web_page.py` & `embedchain-0.1.99/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/xml.py` & `embedchain-0.1.99/embedchain/loaders/xml.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/youtube_channel.py` & `embedchain-0.1.99/embedchain/loaders/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/loaders/youtube_video.py` & `embedchain-0.1.99/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/memory/base.py` & `embedchain-0.1.99/embedchain/memory/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/memory/message.py` & `embedchain-0.1.99/embedchain/memory/message.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/memory/utils.py` & `embedchain-0.1.99/embedchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/migrations/env.py` & `embedchain-0.1.99/embedchain/migrations/env.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/migrations/script.py.mako` & `embedchain-0.1.99/embedchain/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/migrations/versions/40a327b3debd_create_initial_migrations.py` & `embedchain-0.1.99/embedchain/migrations/versions/40a327b3debd_create_initial_migrations.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/models/data_type.py` & `embedchain-0.1.99/embedchain/models/data_type.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/store/assistants.py` & `embedchain-0.1.99/embedchain/store/assistants.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/telemetry/posthog.py` & `embedchain-0.1.99/embedchain/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/utils/cli.py` & `embedchain-0.1.99/embedchain/utils/cli.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/utils/misc.py` & `embedchain-0.1.99/embedchain/utils/misc.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/base.py` & `embedchain-0.1.99/embedchain/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/chroma.py` & `embedchain-0.1.99/embedchain/vectordb/chroma.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/elasticsearch.py` & `embedchain-0.1.99/embedchain/vectordb/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/opensearch.py` & `embedchain-0.1.99/embedchain/vectordb/opensearch.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/pinecone.py` & `embedchain-0.1.99/embedchain/vectordb/pinecone.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/qdrant.py` & `embedchain-0.1.99/embedchain/vectordb/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import os
-import uuid
 from typing import Any, Optional, Union
 
 try:
     from qdrant_client import QdrantClient
     from qdrant_client.http import models
     from qdrant_client.http.models import Batch
     from qdrant_client.models import Distance, VectorParams
```

### Comparing `embedchain-0.1.98/embedchain/vectordb/weaviate.py` & `embedchain-0.1.99/embedchain/vectordb/weaviate.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/embedchain/vectordb/zilliz.py` & `embedchain-0.1.99/embedchain/vectordb/zilliz.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.1.98/pyproject.toml` & `embedchain-0.1.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "embedchain"
-version = "0.1.98"
-description = "Simplest open source retrieval(RAG) framework"
+version = "0.1.99"
+description = "Simplest open source retrieval (RAG) framework"
 authors = [
     "Taranjeet Singh <taranjeet@embedchain.ai>",
     "Deshraj Yadav <deshraj@embedchain.ai>",
 ]
 license = "Apache License"
 readme = "README.md"
 exclude = [
```

### Comparing `embedchain-0.1.98/PKG-INFO` & `embedchain-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.1.98
-Summary: Simplest open source retrieval(RAG) framework
+Version: 0.1.99
+Summary: Simplest open source retrieval (RAG) framework
 License: Apache License
 Author: Taranjeet Singh
 Author-email: taranjeet@embedchain.ai
 Requires-Python: >=3.9,<=3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws-bedrock
 Provides-Extra: cohere
 Provides-Extra: dataloaders
 Provides-Extra: discord
 Provides-Extra: dropbox
 Provides-Extra: elasticsearch
 Provides-Extra: github
```

