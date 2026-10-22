# Awesome-Neural-Search-Frameworks

## Top Neural Search Frameworks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Multimodal Indexing, Cloud-Native Distribution & Vector Retrieval*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Neural Search Frameworks**. These tools enable semantic retrieval across any data type — text, images, video, audio, and code — using deep learning embeddings and vector similarity, rather than relying solely on keyword matching.



**Examples** include Jina, Weaviate, Marqo, Vespa, Haystack, Qdrant, Elasticsearch, Algolia, Coveo, and Amazon Kendra (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, multimodal indexing, and cloud-native distribution — ideal for AI engineers building semantic search applications who want to own their retrieval stack end-to-end without fragmented multi-vendor integrations.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **Algolia** — Developer-favorite hosted search API with instant search, typo tolerance, and **NeuralSearch** for semantic retrieval. **Record-based pricing** scales steeply with catalog size. **Best for site search and e-commerce discovery** where fastest time-to-value matters.



- **Coveo** — AI-powered enterprise search and relevance platform for customer service, workplace, and commerce. Strong connectors for Salesforce, ServiceNow, and legacy systems. **Best for large enterprises** needing unified search across heterogeneous systems.



- **Amazon Kendra** — AWS-managed intelligent enterprise search with natural language queries and connectors to S3, SharePoint, Salesforce, and databases. **Best for AWS-native organizations** wanting managed neural search without infrastructure.



## Open-Source GitHub Projects



- **[Jina](https://github.com/jina-ai/jina)**  

  **The cloud-native neural search framework for any kind of data** — Apache 2.0 licensed . **Empowers anyone to build SOTA and scalable deep learning search applications in minutes** . **All data types supported**: scalable indexing, querying, and understanding of video, image, long/short text, music, source code, PDF, and more . **Three fundamental concepts**: **Document** (basic data type), **Executor** (how Documents are processed), and **Flow** (how Executors are streamlined and distributed) . **Fast & cloud-native by design**: distributed architecture from day one with containerizing, streaming, paralleling, sharding, async scheduling, and HTTP/gRPC/WebSocket protocols . **Own your stack** — keep end-to-end ownership and avoid integration pitfalls from fragmented multi-vendor legacy tools . **Install via PyPI, Conda, or Docker** (80MB universal container image for multiple architectures) . **Quick demos**: `jina hello fashion` (image search), `jina hello chatbot` (QA), `jina hello multimodal` (multimodal search) . **Best for teams wanting a complete, cloud-native framework for building multimodal neural search applications** from prototype to production.



- **[Weaviate](https://github.com/weaviate/weaviate)**  

  **The cloud-native, real-time vector search engine** — BSD-3-Clause licensed, **14,500+ GitHub stars** . **Stores both objects and vectors**, allowing combination of vector search with structured filtering with fault tolerance and scalability of a cloud-native database . **Accessible through GraphQL, REST, and various language clients** . **Extensions for specific use cases** such as semantic search, plugins to integrate in any application, and a console to visualize data . **Keywords**: vector search engine, neural search engine, semantic search, HNSW, deep search, kNN . **Best for teams wanting a production-grade vector database with hybrid search and structured filtering.**



- **[Marqo](https://github.com/marqo-ai/marqo)**  

  **The tensor search engine for humans** — Apache 2.0 licensed, **4,900+ GitHub stars** . **Unified embedding generation and search engine** that seamlessly integrates into applications, web pages, and workflows . **Tensor search** transforms documents, images, and other data into vector collections, enabling human-like matching of search requests to files . **Use cases**: user search and recommendation systems, multimodal search (image-to-image, text-to-image, image-to-text), chatbots, and text/image classification . **Quick start via Docker**: `docker run --name marqo -it --privileged -p 8882:8882 marqoai/marqo` then `pip install marqo` . **Client API**: `mq.index("my-first-index").add_documents([...])` and `mq.index("my-first-index").search(q="...")` . **Supports lexical search and field-specific search** alongside tensor search . **Best for teams wanting an easy-to-use tensor search engine** with multimodal capabilities and a simple Python client.



- **[Vespa](https://github.com/vespa-engine/vespa)**  

  **The AI search platform with native tensor and ML inference** — Apache 2.0 licensed . **Vector search with HNSW indexes**, **BM25 text search and hybrid search**, and **native tensor and ML model inference at serving time** . **YQL (Vespa Query Language)** for structured queries, **multi-phase ranking** (match-phase, first-phase, second-phase, global-phase), and **real-time indexing with sub-100ms query latency** . **Distributed content clusters** with automatic sharding and replication . **Built-in machine learning inference** (TensorFlow, ONNX, XGBoost, LightGBM) . **Self-managed (Apache 2.0) or fully managed Vespa Cloud** (AWS, GCP) with startup plans from $0.05/vCPU-hour . **Best for teams needing advanced ranking and ML inference at serving time** — the most feature-complete open-source search platform for complex relevance requirements.



- **[Haystack](https://github.com/deepset-ai/haystack)**  

  **The open-source AI orchestration framework for context-engineered LLM applications** — Apache 2.0 licensed . **Design modular pipelines and agent workflows with explicit control over retrieval, routing, memory, and generation** . **Built for scalable agents, RAG, multimodal applications, semantic search, and conversational systems** . **Document Stores** connect to Qdrant, Weaviate, Elasticsearch, OpenSearch, Pinecone, Chroma, Milvus, pgvector, and more . **Hybrid retrieval** via `DocumentJoiner` with reciprocal rank fusion, combining dense embeddings with sparse BM25 . **Hayhooks** turns pipelines into self-hosted REST APIs with one command . **Best for teams wanting explicit, type-safe pipeline composition** with predictable execution and swappable retrieval backends.



- **[Qdrant](https://github.com/qdrant/qdrant)**  

  **The leading open-source vector database for filter-heavy neural search** — Apache 2.0 licensed . **Native hybrid search** — dense vector plus BM25 sparse via RRF fusion using built-in fastembed integration . **Payload-aware HNSW traversal** applies filters during graph traversal, not after — sub-millisecond latency on predicated queries . **Best for neural search requiring metadata filtering** on retrieval.



- **[Elasticsearch](https://github.com/elastic/elasticsearch)**  

  **The most widely deployed search engine with vector and hybrid support** — SSPL/Elastic License 2.0 (not OSI-approved) . **Vector search with HNSW**, hybrid BM25 + kNN, and **semantic_text** for managed embeddings . **Built on Lucene**, which itself includes HNSW indexing and search capabilities since version 9 . **Best for teams already on Elastic** wanting neural search alongside traditional search and log analytics.



### Additional Strong Open-Source Options



- **Lucene** — The underlying search library powering Elasticsearch, OpenSearch, and Solr. **HNSW indexing and search capabilities** since version 9, meaning dedicated vector stores differ primarily in performance, not must-have features . Best for teams wanting to avoid introducing a separate vector store into an already complex stack.

- **OpenSearch** — Apache 2.0 licensed fork of Elasticsearch with Neural Search plugin for vector search and hybrid retrieval. Best for teams requiring OSI-approved licensing.

- **FAISS** — Facebook's library for efficient similarity search and clustering. The foundational ANN library many vector databases build on.

- **USearch** — Smaller and faster single-file similarity search engine with bindings for multiple languages.



**Frameworks for building custom systems**: Combine **Jina** for cloud-native multimodal neural search with any data type, **Weaviate** for production vector search with hybrid filtering, **Marqo** for simple tensor search with multimodal capabilities, **Vespa** for advanced ranking and ML inference at serving time, **Haystack** for explicit pipeline composition with swappable backends, and **Qdrant** for filter-heavy vector retrieval — to build a neural search stack tailored to your data modalities, ranking complexity, and deployment constraints.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Neural search frameworks differ significantly in data modality support, ranking sophistication, and operational complexity. **Jina is the most complete cloud-native framework** for building multimodal search from scratch, but its Flow/Executor architecture requires understanding distributed concepts . **Weaviate and Qdrant are vector databases** — they store and retrieve vectors but expect you to handle embedding generation upstream . **Marqo simplifies the full pipeline** with built-in embedding and a simple Python client, trading some flexibility for ease of use . **Vespa is the most powerful for complex ranking** with multi-phase ranking and native ML inference, but has the steepest learning curve . **Haystack is a pipeline framework**, not a search engine itself — it orchestrates retrieval components . **Lucene-based systems (Elasticsearch, OpenSearch, Solr) already have HNSW vector search** — evaluate whether a dedicated vector store adds enough value to justify the operational overhead .

- Self-hosted open-source solutions require proper embedding model selection, vector dimension configuration, and retrieval quality evaluation against ground truth.



---



**Made for AI engineers, search architects, and teams building neural search applications across text, images, and multimodal data.**

Let's make neural search more open, multimodal, and retrieval-accurate.
