# Fu Dai

Data Scientist with a production engineering side. I work on AI systems that
have to run reliably at inference time — not just in notebooks.

Current focus: multimodal AI serving (TTS, OCR, LLM) on GPU infrastructure.

## Production serving systems

Three repos with real benchmark data on A100 / H200:

| Repo | What it does |
|------|-------------|
| [vllm-chatterbox-stream](https://github.com/wuxuedaifu/vllm-chatterbox-stream) | Multilingual TTS on vLLM — ~0.7s TTFB, 23 languages, voice cloning, OpenAI-compatible |
| [vllm-surya-ocr](https://github.com/wuxuedaifu/vllm-surya-ocr) | OCR serving with vLLM — 9.5× speedup via CUDA graphs, concurrency sweep tested |
| [xttsv2-vllm-streaming-server](https://github.com/wuxuedaifu/xttsv2-vllm-streaming-server) | XTTS-v2 real-time streaming — ~0.5s TTFB, Docker, GPU serving |

All three expose OpenAI-compatible APIs and ship with Docker.

## Data science work

- **ASR / TTS**: speech systems, streaming inference, latency optimization
- **Vision**: OCR, face recognition, document AI
- **LLM**: RAG pipelines, serving infra, OpenAI-compatible APIs
- **Data**: ClickHouse, PostgreSQL, ETL pipelines, AQI/weather data systems

## Stack

Python · vLLM · FastAPI · CUDA · Docker · Kubernetes  
ClickHouse · PostgreSQL · Java · SQL
