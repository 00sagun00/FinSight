# FinSight RAG

FinSight RAG is a Streamlit app for asking questions about financial reports. It indexes PDFs with Sentence Transformers and FAISS, then retrieves relevant passages to help generate answers.

## Run locally

```bash
cd finsight-rag
python -m venv .venv
pip install -r requirements.txt
```

Add PDF reports to `data/`, build the index, and start the app:

```bash
python embeddings/embed_store_faiss.py
streamlit run app.py
```
