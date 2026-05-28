# CyberRAG

CyberRAG is a Streamlit app that lets you build a RAG (Retrieval-Augmented Generation) 
pipeline from any data source using natural language — no complex setup required.

## What You Can Do
1. Describe your data source (local file or web page) and your task
2. Configure RAG parameters (top-k, chunk size, summarization, etc.)
3. Query your data through a conversational chat interface

## Installation

Clone the repo and navigate into the project folder:

```bash
git clone https://github.com/gajulapallisubramanyam-svg/CyberRAG.git
cd CyberRAG
python3 -m venv .venv
source .venv/bin/activate
poetry install
```

Add your API key in `.streamlit/secrets.toml`:

```toml
openai_key = "<your_openai_key>"
```

Run the app:

```bash
streamlit run 1_🏠_Home.py
```

## How It Works

| Section | Description |
|---|---|
| 🏠 Home | Build your RAG pipeline by describing your dataset and task |
| ⚙️ RAG Config | View and edit generated parameters (top-k, chunk size, LLM, etc.) |
| 🤖 RAG Agent | Chat with your data using the configured agent |

## Supported LLMs & Embeddings

- **OpenAI** — `openai:gpt-4-1106-preview`
- **Anthropic** — `anthropic:claude-2`
- **Replicate** — `replicate:<model_name>`
- **HuggingFace (local)** — `local:BAAI/bge-small-en`

Embeddings default to `text-embedding-ada-002`. HuggingFace models supported with `local:` prefix.

## Resources

- Built with [LlamaIndex](https://github.com/run-llama/llama_index)
- Issues? Open a [GitHub Issue](https://github.com/gajulapallisubramanyam-svg/CyberRAG/issues) 
or join our [Discord](https://discord.gg/dGcwcsnxhU)
