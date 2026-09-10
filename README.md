# Roei Mashraki

**I build model evaluation tooling for ML teams**, along with the data pipelines and cloud infrastructure it runs on.
Python, FastAPI, PostgreSQL, AWS. Israel. **Open to backend and AI infrastructure roles.**

2.5 years doing this in production at an AI startup, and building it in the open since. VisionDiff below is the current version of the same idea.

[LinkedIn](https://www.linkedin.com/in/roei-mashraki/) · mashraki.work@gmail.com

---

## VisionDiff

[github.com/mashrakiwork/VisionDiff](https://github.com/mashrakiwork/VisionDiff)

A/B regression testing for vision-language models. Run a baseline and a candidate over the same dataset through LM Studio and get a statistical verdict instead of a vibe.

- Returns Improvement, Regression or No Change from a 95% confidence interval using paired seeded bootstrap, with an exact McNemar test over the samples the two models disagreed on
- Deterministic offline scorers (exact match, ANLS, relaxed chart accuracy, token and n-gram F1, field-level F1, IoU) across OCR, document VQA, chart QA, counting, captioning and JSON extraction
- Content-hashed datasets and seeded runs, so results reproduce. CI regenerates every dataset to prove it
- Test suite runs with no GPU and no network

`Python 3.12` `FastAPI` `SQLAlchemy 2.0` `React 19` `TypeScript` `NVML`

## Slice Overflow

[github.com/mashrakiwork/Pizzeria-Slice-Overflow](https://github.com/mashrakiwork/Pizzeria-Slice-Overflow)

Full-stack ordering platform built to production conventions.

- Four sign-in paths on one account model, including Google and Apple over OpenID Connect, with ID tokens verified against each provider's JWKS rather than merely decoded
- Server-authoritative pricing. Deals carry conditions (minimum basket, matching-item count, daypart) and coupons apply after deals, so discounts never compound by accident
- Hebrew and RTL storefront built on CSS logical properties rather than duplicate components, multi-currency pricing from live ECB rates, and live order tracking derived as a pure function of time
- pytest tests, Dockerized Postgres, Alembic migrations

`Python 3.12` `async FastAPI` `PostgreSQL` `React 19` `Stripe` `Docker`

## DepthConverter

[github.com/mashrakiwork/DepthConverter](https://github.com/mashrakiwork/DepthConverter)

Offline 2D to 3D SBS conversion for VR headsets. Upscaling, monocular depth estimation and GPU stereo synthesis in one local pipeline, no cloud uploads.

- Hardware detection with VRAM-based batch sizing and FP16 inference that falls back automatically on out-of-memory
- Frames stream through ffmpeg pipes, so RAM stays constant regardless of video length
- Depth Anything V3 and V2, MiDaS and DPT presets, plus any custom Hugging Face repo

`Python 3.12` `PyTorch CUDA` `PySide6` `FFmpeg (x265, NVENC)` `uv`

## Also building

**StockAssistant** market data and technical-indicator engine with backtesting, plus work that is not public yet.

## Stack

**Backend** Python, SQL, FastAPI, asyncio, SQLAlchemy, Pydantic, Alembic, PostgreSQL, MongoDB, REST APIs, OAuth 2.0 and OpenID Connect<br>
**Cloud** AWS (S3, CloudWatch, SQS), Docker, pytest, Git, GitLab CI/CD<br>
**Applied AI** local LLM inference for coding (Qwen, DeepSeek, Gemma), model benchmarking and evaluation, PyTorch, LoRA training (ai-toolkit), ComfyUI, Hugging Face, Claude and Codex, generative image/video/3D (Wan, LTX, MiniMax, Tripo3D)<br>
**Frontend** React, TypeScript, Tailwind CSS, Vite, Java

---

<img alt="Breakout" src="https://raw.githubusercontent.com/mashrakiwork/mashrakiwork/github-breakout/images/breakout.svg" />
