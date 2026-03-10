# Local AI

A single-file local AI chat UI powered by [Ollama](https://ollama.com). Multi-modal, chat history, no install.

## Setup

```bash
# Start Ollama with CORS enabled (required)
OLLAMA_ORIGINS=* ollama serve
```

Then open `index.html` in your browser.

## Models

### By PC specs

| RAM | Recommended |
|-----|-------------|
| 4–6 GB | `deepseek-r1:1.5b`, `llama3.2:3b` |
| 8 GB | `deepseek-r1:3b`, `llama3.2`, `mistral` |
| 16 GB | `deepseek-r1:8b`, `llama3.1:8b` |
| 32 GB+ | `deepseek-r1:14b`, `llama3.1:70b` (GPU recommended) |

### By use-case

| Use-case | Model |
|----------|-------|
| Images / vision | `llava` |
| Coding & reasoning | `deepseek-r1:3b` (fast) · `deepseek-r1:8b` (better) |
| General chat | `llama3.2` · `mistral` |
| Fastest responses | `deepseek-r1:1.5b` · `llama3.2` |

### Pull a model

```bash
ollama pull llava            # vision (images)
ollama pull deepseek-r1:3b   # good all-rounder
ollama pull llama3.2         # fast general chat
```
