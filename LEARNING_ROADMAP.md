# Learning Roadmap

## Phase 1 — Foundations
- [ ] Explain one-hot vectors and their limitations.
- [ ] Compute dot product, vector norm, and cosine similarity by hand.
- [ ] Explain why cosine similarity is not a probability.

## Phase 2 — Retrieval
- [ ] Store at least 20 documents in ChromaDB.
- [ ] Add source and topic metadata.
- [ ] Test 10 queries and record whether the expected document appears in the top 3.
- [ ] Try multiple chunk sizes and inspect boundary cases.

## Phase 3 — RAG mini-project
- [ ] Load a small set of authorized PDF/text documents.
- [ ] Chunk documents and retain source/page metadata.
- [ ] Embed chunks and retrieve top-k passages for a query.
- [ ] Send retrieved context to an LLM of your choice.
- [ ] Display citations/source names with each answer.
- [ ] Evaluate groundedness with questions whose answers are and are not in the documents.

## Portfolio deliverables
- Clear README with setup and screenshots.
- A small evaluation table of query, expected source, retrieved source, and outcome.
- A short limitations section describing hallucination risk and retrieval misses.
