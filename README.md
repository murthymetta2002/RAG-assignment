# RAG Assignment: Baseline vs. Re-Ranking

Compares bi-encoder retrieval against bi-encoder + cross-encoder re-ranking over the Gloomhaven rulebook.

## Run

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
$env:GEMINI_API_KEY = "<your key>"
```

Place the rulebook PDF at `data/gloomhaven_rulebook.pdf`, then run `rag_rerank.ipynb` top to bottom.

## Models

- Bi-encoder: `sentence-transformers/all-MiniLM-L6-v2`
- Cross-encoder: `cross-encoder/ms-marco-MiniLM-L-6-v2`
- LLM: Gemini (model name set in the notebook config)
