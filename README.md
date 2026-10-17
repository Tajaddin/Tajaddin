# Tajaddin Gafarov

AI and software engineer in Tampa, FL. M.S. in Computer Science at the University of South Florida, expected May 2027; B.S. in Computer Science, USF, May 2025. Since 2021 I have built ML and data systems for two companies, remotely and part-time alongside full-time study.

Every repository below ships with tests and a measured result. Unless marked otherwise, the numbers were reproduced from a fresh clone on 2026-10-16.

Website and resume: [tajaddin.github.io](https://tajaddin.github.io) · [LinkedIn](https://www.linkedin.com/in/tajaddin-gafarov) · gafarovtajaddin@gmail.com

## Featured

| Project | What it is | Measured result |
|---|---|---|
| [code-fix-agent](https://github.com/Tajaddin/code-fix-agent) | Agent on the Anthropic API that reproduces, patches and verifies Python bugs in a pytest-driven loop, one isolated workspace per attempt | **12/12 bugs fixed** live on Claude Haiku 4.5, 3.58 iterations per bug, $0.10 total (committed live run; mock pipeline re-run) |
| [langgraph-research-pilot](https://github.com/Tajaddin/langgraph-research-pilot) | LangGraph RAG agent for Wikipedia QA with citations, multi-query retrieval, a fact-check step, human-in-the-loop gates and crash-resumable state | **F1 0.313 to 0.368 (+17% relative)** over a single-prompt baseline on 30 HotpotQA questions, Claude Haiku 4.5 (committed run) |
| [streaming-etl-pipeline](https://github.com/Tajaddin/streaming-etl-pipeline) | Event-time ETL into DuckDB with per-partition watermarks, late-data side outputs and crash-safe checkpoints | **0% false-late events vs 71%** with a single global watermark; 25 tests |
| [fake-news-detector-ml](https://github.com/Tajaddin/fake-news-detector-ml) | A six-step data audit that traced a 99 to 100% baseline to publisher and stylistic leakage, then the honest number | **62.1% accuracy, 0.676 ROC-AUC** on the 1,267-statement LIAR test set; 25 tests |
| [webhook-delivery](https://github.com/Tajaddin/webhook-delivery) | At-least-once delivery with exponential backoff, a dead-letter queue, HMAC signing and idempotency keys | **99.92% eventual delivery** under 30% injected transient failures in a deterministic fault-injection benchmark (virtual clock, no network); 21 tests |
| [go-grpc-kvstore](https://github.com/Tajaddin/go-grpc-kvstore) | In-memory key-value store over gRPC and REST with TTL, a streaming Watch and sharded concurrency | **~51,800 ops/s at p99 2.84 ms** on the Get path over real gRPC (re-run here: ~104,000 ops/s, p99 1.4 ms); 16 race-detector tests |

## More

- [medrag-ground](https://github.com/Tajaddin/medrag-ground): audit-logged RAG over OpenFDA drug labels. 200-question eval: 100% refusal on unanswerable, PII and adversarial prompts, 90% citation rate, 0 hallucinated drug names (committed live run).
- [mcp-server-toolkit](https://github.com/Tajaddin/mcp-server-toolkit): framework for Model Context Protocol servers with three example servers and an in-memory test harness; p99 tool round trip 8.2 ms.
- [multi-agent-supervisor](https://github.com/Tajaddin/multi-agent-supervisor): planner, retriever, analyzer, verifier and synthesizer agents run in parallel; 1.31x faster than sequential on a 5-question HotpotQA run, 1.99x in a simulated-latency benchmark.
- [kafka-clickhouse-analytics](https://github.com/Tajaddin/kafka-clickhouse-analytics): Kafka to tumbling-window aggregation to ClickHouse; 931K events/s on one core in the README, 2.39M/s re-run.
- [spring-boot-task-api](https://github.com/Tajaddin/spring-boot-task-api), [aspnetcore-inventory-api](https://github.com/Tajaddin/aspnetcore-inventory-api), [ktor-url-shortener](https://github.com/Tajaddin/ktor-url-shortener): JWT, EF Core and Ktor services with load probes. READMEs say 973, 1,482 and ~1,500 req/s; re-run on an i7 they gave 2,500, 3,200 and 3,200 req/s at p99 under 45 ms.
- [cuda-inlj](https://github.com/Tajaddin/cuda-inlj): GPU index nested-loop join with a B+ tree. The probe kernel is 4.4x faster than a GPU hash-join kernel; a separator-key bug that silently dropped 1.5% of matches is fixed.
- [llm-knowledge-editing](https://github.com/Tajaddin/llm-knowledge-editing): reproduction of the ACL 2024 "Learning to Edit" paper on LLaMA2-Chat-7B, with a 12-page report documenting three discrepancies from the published results.
- [reproduce-stepback](https://github.com/Tajaddin/reproduce-stepback): an ICLR 2024 prompting paper's +5.5-point gain falls to +0.0 on Claude Haiku 4.5, because the model saturates the benchmark. A negative result, reported as one.

## Stack

Python, SQL, Go, TypeScript, Java, Kotlin, C#, C/C++ · PyTorch, scikit-learn, Hugging Face, XGBoost, MLflow, LangChain, LangGraph, Anthropic API, MCP · Kafka, ClickHouse, DuckDB, PostgreSQL, MongoDB, Redis, Spark, Airflow · FastAPI, Spring Boot, ASP.NET Core, gRPC, React · AWS, GCP, Docker, Kubernetes, Terraform, GitHub Actions

Open to new-grad and early-career AI, ML, data and software engineering roles in Tampa Bay or remote US. Authorized to work in the US, no sponsorship needed.
