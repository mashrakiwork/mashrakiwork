# Roei Mashraki

**Backend engineer working on model evaluation, data pipelines and cloud infrastructure.**
Python, FastAPI, PostgreSQL, AWS. Based in Ra'anana, Israel. **Open to backend and AI infrastructure roles.**

I build the systems that test whether ML models actually work. Previously 2.5 years at an AI startup detecting counterfeit and defective electronic components on production lines, where I built the ML team's model evaluation tooling.

[LinkedIn](https://www.linkedin.com/in/roei-mashraki/) · mashraki.work@gmail.com

---

## VisionDiff

[github.com/mashrakiwork/VisionDiff](https://github.com/mashrakiwork/VisionDiff)

A/B regression testing for vision-language models. Run a baseline and a candidate over the same dataset through LM Studio and get a statistical verdict instead of a vibe.

- Returns Improvement, Regression or No Change from a 95% confidence interval using paired seeded bootstrap, with an exact McNemar test over the samples the two models disagreed on
- Nine deterministic offline scorers (exact match, ANLS, relaxed chart accuracy, token and n-gram F1, field-level F1, IoU) across OCR, document VQA, chart QA, counting, captioning and JSON extraction
- Content-hashed datasets and seeded runs, so results reproduce. CI regenerates every dataset to prove it
- Test suite runs with no GPU and no network

`Python 3.12` `FastAPI` `SQLAlchemy 2.0` `React 19` `TypeScript` `NVML`

## Slice Overflow

[github.com/mashrakiwork/Pizzeria-Slice-Overflow](https://github.com/mashrakiwork/Pizzeria-Slice-Overflow)

Full-stack ordering platform built to production conventions.

- Four sign-in paths on one account model, including Google and Apple over OpenID Connect, with ID tokens verified against each provider's JWKS rather than merely decoded
- Server-authoritative pricing. Deals carry conditions (minimum basket, matching-item count, daypart) and coupons apply after deals, so discounts never compound by accident
- Hebrew and RTL storefront built on CSS logical properties rather than duplicate components, four-currency pricing from live ECB rates, and live order tracking derived as a pure function of time
- 113 pytest tests, Dockerized Postgres, Alembic migrations

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

**Backend** Python, FastAPI, async SQLAlchemy, Pydantic, PostgreSQL, MongoDB, OAuth 2.0 and OpenID Connect
**Cloud** AWS (S3, CloudWatch, SQS), Docker, Git, CI/CD
**Applied AI** local LLM and VLM inference (LM Studio), model benchmarking and evaluation, PyTorch, LoRA training (ai-toolkit), ComfyUI, Anthropic and DeepSeek APIs
**Also** React, TypeScript, Rust, Java

---

<img alt="Breakout" src="https://raw.githubusercontent.com/mashrakiwork/mashrakiwork/github-breakout/images/breakout.svg" />
