# Project Guide: GenAI and RAG

## Decide before coding
- Define the task and how answer quality will be measured.
- Choose a model provider; verify current model availability, pricing, rate limits, and data policy.
- Select a compatible embedding model and verify vector dimensions.
- Decide how documents are parsed, cleaned, chunked, embedded, indexed, updated, and removed.
- Choose a vector store based on scale, filtering, operations, hosting, and cost.
- Decide whether citations, access controls, evaluation, and audit logs are required.
- Set latency, reliability, and quality targets.
- Plan for prompt injection and untrusted documents.

## Architecture
Show ingestion separately from query-time retrieval. Include parsing, chunking, embeddings, indexing, retrieval, reranking if used, generation, citations, and persistence.

## Reliability and safety
- Treat retrieved documents as untrusted data, not instructions.
- Restrict document access to authorized users.
- Handle provider errors, rate limits, timeouts, empty retrieval, and malformed output.
- Verify model capabilities from official documentation; do not assume every provider supports embeddings.
- Use representative evaluations; a successful API call does not prove answer quality.
- Keep secrets out of prompts, logs, and repositories.
