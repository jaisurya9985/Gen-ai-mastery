# GenAI Learning Lab — Original Study Pack

A fresh, hands-on learning path covering text representations, vector geometry, vector databases, document chunking, and semantic retrieval. This project was created as an independent alternative study pack inspired by the *topics* in the reference repository; the notebook explanations, sample datasets, naming, and exercises here are newly written.

## Learning path

1. `01_embeddings_from_scratch.ipynb` — one-hot vectors and representation intuition.
2. `02_similarity_and_search.ipynb` — cosine similarity, ranking, and edge cases.
3. `03_vector_store_chromadb.ipynb` — semantic retrieval, metadata filtering, persistence.
4. `04_chromadb_data_management.ipynb` — create/read/update/upsert/delete operations.
5. `05_rag_document_ingestion.ipynb` — document loading, chunking, and source metadata.
6. `06_huggingface_semantic_search.ipynb` — real embeddings and a semantic search function.

## Run locally

Recommended: Python 3.10 or 3.11 in a virtual environment.

```bash
python -m venv .venv
# Windows PowerShell:
.venv\Scripts\Activate.ps1
# macOS/Linux:
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter lab
```

Open the notebooks in order. Some notebooks contain `%pip` cells that install their own focused dependencies. The Hugging Face notebook downloads model weights on first use. Chroma persistence creates a local `local_vector_data/` directory.

## Google Colab

Upload the notebook you want to run to Google Colab. Run the cells from top to bottom. The sample documents are generated inside the notebook so the document-ingestion example does not require an external dataset.

## Notes

- The examples are educational demonstrations, not a production RAG system.
- Similarity scores are ranking signals, not calibrated probabilities.
- Inspect retrieved passages and test with realistic questions before using a system for consequential decisions.
- Never commit API keys, private documents, or credentials to a public repository.

## Suggested extensions

- Add PDF ingestion and per-page citations.
- Persist embeddings and implement a small RAG answer function.
- Evaluate retrieval with a set of query/expected-document pairs.
- Add a Streamlit UI and deploy it after checking model download size and hosting limits.
