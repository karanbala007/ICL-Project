# ICL-Project

This project contains a simple end-to-end RAG workflow inspired by the GENAI assessment notebooks.

## Included notebooks

1. `RAG_Step1_Document_Loading_and_Chunkin.ipynb` - loads source documents and splits them into chunks.
2. `RAG_Step2_Storing_Chunks_in_ChromaDB.ipynb` - stores chunked text in ChromaDB.
3. `RAG_Step3_Retrieving_Relevant_Context.ipynb` - retrieves the most relevant chunks for a query.
4. `RAG_Step4_Passing_Context_to_Gemini_Groq_LLM.ipynb` - sends the retrieved context to an LLM for answer generation.

## Suggested setup

Install the required Python packages before running the notebooks:

```bash
pip install chromadb sentence-transformers python-dotenv google-generativeai requests
```

For the final LLM step, set one of the following environment variables:

```bash
export GROQ_API_KEY="your_groq_api_key"
# or
export GEMINI_API_KEY="your_gemini_api_key"
```

These notebooks are intentionally beginner-friendly and can be used as a practical RAG reference for learning and assessment work.
