# Roei Mashraki

Backend engineer with 2.5 years at an AI startup, building FastAPI services, evaluation tooling, and data workflows.<br> Since 2023, developing independent backend and AI projects focused on reliable testing, automation, and production-ready workflows.

**Open to backend and AI infrastructure roles.**

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

## Technical Skills

**Backend** Python, SQL, FastAPI, asyncio, SQLAlchemy, Pydantic, Alembic, REST APIs, OAuth 2.0<br>
**Data & delivery** PostgreSQL, MongoDB, AWS (S3, CloudWatch, SQS), Docker, pytest, Git, GitLab CI/CD<br>
**AI tooling** Claude, Codex, Hugging Face, ComfyUI, LoRA training (ai-toolkit), local LLM inference for coding (Qwen, DeepSeek, Gemma). Generative image, video and 3D models (Wan, LTX, MiniMax, Tripo3D).<br>
**Frontend** TypeScript, React, Tailwind CSS, Vite

---

<img alt="Breakout" src="https://raw.githubusercontent.com/mashrakiwork/mashrakiwork/github-breakout/images/breakout.svg" />
