# Fu Dai

Data Scientist with a production engineering side. I work on AI systems that
have to run reliably at inference time — not just in notebooks.

Current focus: multimodal AI serving (TTS, OCR, ASR, LLM) on GPU infrastructure.

## Production serving systems

vLLM-based serving repos with real benchmark data on A100 / H200:

| Repo | What it does |
|------|-------------|
| [vllm-chatterbox-stream](https://github.com/wuxuedaifu/vllm-chatterbox-stream) | Multilingual TTS on vLLM — ~0.7s TTFB, 23 languages, voice cloning, OpenAI-compatible |
| [Kokoro-vllm](https://github.com/wuxuedaifu/Kokoro-vllm) | Kokoro-82M TTS on vLLM V1 — ~89ms TTFB, ~48× real-time (H200), bit-exact parity, OpenAI-compatible |
| [xttsv2-vllm-streaming-server](https://github.com/wuxuedaifu/xttsv2-vllm-streaming-server) | XTTS-v2 real-time streaming TTS — ~0.5s TTFB, Docker, GPU serving |
| [vllm-surya-ocr](https://github.com/wuxuedaifu/vllm-surya-ocr) | OCR serving with vLLM — 9.5× speedup via CUDA graphs, concurrency sweep tested |
| [Canary-Qwen-2.5b-vllm](https://github.com/wuxuedaifu/Canary-Qwen-2.5b-vllm) | Canary-Qwen-2.5B ASR (SALM) on vLLM — fixes long-audio RoPE truncation bug, verified vs NeMo on H200 |

All expose OpenAI-compatible APIs and ship with Docker.

## Data science work

- **ASR / TTS**: speech systems, streaming inference, latency optimization
- **Vision**: OCR, face recognition, document AI
- **LLM**: RAG pipelines, serving infra, OpenAI-compatible APIs
- **Data**: ClickHouse, PostgreSQL, ETL pipelines, AQI/weather data systems

## Stack

Python · vLLM · FastAPI · CUDA · Docker · Kubernetes  
ClickHouse · PostgreSQL · Java · SQL
