# Awesome MLX [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome projects, tools, models, and resources for [Apple MLX](https://github.com/ml-explore/mlx) — the ML framework for Apple Silicon.

**Run AI models on your Mac at full speed.** This list covers everything built on MLX — inference servers, training tools, audio/speech/vision models, Swift packages, and more. Whether you want a ChatGPT-like experience offline or you're building an AI app, start here.

## Why MLX?

MLX is Apple's open-source ML framework designed for Apple Silicon. If you have an M1/M2/M3/M4 Mac:

- **Use all your RAM for models** — Your Mac's memory is shared between CPU and GPU. A 32GB Mac can run a 30GB model — no copying between chips.
- **Faster than CUDA workarounds** — Native Metal GPU acceleration, not a compatibility layer.
- **Growing fast** — 120+ projects, 2000+ optimized models on HuggingFace, and active community.

## Quick Start

**"I just want to chat with a local AI on my Mac"**
→ Install [Klee](https://github.com/signerlabs/Klee) (native app, one click) or [chat-with-mlx](https://github.com/qnguyen3/chat-with-mlx) (web UI)

**"I want an OpenAI-compatible local API server"**
→ Install [Rapid-MLX](https://github.com/raullenchai/Rapid-MLX) (`pip install vllm-mlx && rapid-mlx serve qwen3.5-9b`)

**"I want to fine-tune a model on my Mac"**
→ Use [mlx-tune](https://github.com/ARahim3/mlx-tune) (SFT, DPO, GRPO) or Apple's built-in [mlx-lm](https://github.com/ml-explore/mlx-lm) LoRA

**"I'm building a Swift/iOS app with on-device AI"**
→ Start with [mlx-swift-lm](https://github.com/ml-explore/mlx-swift-lm) + [fullmoon-ios](https://github.com/mainframecomputer/fullmoon-ios) as reference

**[Submit your project →](#contributing)** PRs and issues welcome! Language legend: 🐍 Python · 🦅 Swift · 🟨 JS/TS · 🦀 Rust · 🐹 Go

---

## Contents

- [Core Framework](#core-framework)
- [Inference & Serving](#inference--serving)
- [Training & Fine-tuning](#training--fine-tuning)
- [Audio & Speech](#audio--speech)
- [Image & Video Generation](#image--video-generation)
- [Vision & Multimodal](#vision--multimodal)
- [Embeddings & RAG](#embeddings--rag)
- [Swift Ecosystem](#swift-ecosystem)
- [Benchmarks](#benchmarks)
- [Apps & Demos](#apps--demos)
- [Other Tools](#other-tools)
- [Models](#models)
- [Learning Resources](#learning-resources)

---

## Core Framework

- 🐍 [mlx](https://github.com/ml-explore/mlx) — Apple's array framework for ML on Apple silicon. The foundation. ![](https://img.shields.io/github/stars/ml-explore/mlx?style=flat-square)
- 🐍 [mlx-examples](https://github.com/ml-explore/mlx-examples) — Official examples: LLMs, LoRA, Stable Diffusion, Whisper, and more. ![](https://img.shields.io/github/stars/ml-explore/mlx-examples?style=flat-square)
- 🐍 [mlx-lm](https://github.com/ml-explore/mlx-lm) — Apple's official LLM runner. Text generation, quantization, LoRA. ![](https://img.shields.io/github/stars/ml-explore/mlx-lm?style=flat-square)
- 🦅 [mlx-swift](https://github.com/ml-explore/mlx-swift) — Swift API for MLX. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift?style=flat-square)
- 🦅 [mlx-swift-examples](https://github.com/ml-explore/mlx-swift-examples) — Examples using MLX Swift: LLMs, image generation, training. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift-examples?style=flat-square)
- 🦅 [mlx-swift-lm](https://github.com/ml-explore/mlx-swift-lm) — LLMs and VLMs with MLX Swift. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift-lm?style=flat-square)
- 🟨 [node-mlx](https://github.com/frost-beta/node-mlx) — Machine learning framework for Node.js, built on MLX. ![](https://img.shields.io/github/stars/frost-beta/node-mlx?style=flat-square)
- 🐍 [mlx-data](https://github.com/ml-explore/mlx-data) — Apple's efficient framework-agnostic data loading. ![](https://img.shields.io/github/stars/ml-explore/mlx-data?style=flat-square)
- 🐍 [mlx-c](https://github.com/ml-explore/mlx-c) — Official C API for MLX. ![](https://img.shields.io/github/stars/ml-explore/mlx-c?style=flat-square)
- 🦀 [mlx-rs](https://github.com/oxiglade/mlx-rs) — Unofficial Rust bindings to Apple's MLX framework. ![](https://img.shields.io/github/stars/oxiglade/mlx-rs?style=flat-square)
- 🐍 [mlx-graphs](https://github.com/mlx-graphs/mlx-graphs) — Graph Neural Network library for Apple Silicon. ![](https://img.shields.io/github/stars/mlx-graphs/mlx-graphs?style=flat-square)
- [emlx](https://github.com/elixir-nx/emlx) — MLX backend for Elixir Nx. ![](https://img.shields.io/github/stars/elixir-nx/emlx?style=flat-square)
- [ocaml-mlx](https://github.com/ocaml-mlx/mlx) — OCaml bindings for MLX with JSX syntax. ![](https://img.shields.io/github/stars/ocaml-mlx/mlx?style=flat-square)

## Inference & Serving

> **Which one should I use?** Quick guide:
> - **Just want a GUI app?** → [omlx](https://github.com/jundot/omlx) (menu bar) or [LM Studio](https://lmstudio.ai) (desktop app)
> - **Need an OpenAI-compatible API?** → [Rapid-MLX](https://github.com/raullenchai/Rapid-MLX) (fastest, tool calling) or [mlx-omni-server](https://github.com/madroidmaq/mlx-omni-server)
> - **Building a Swift/iOS app?** → [swama](https://github.com/Trans-N-ai/swama) or [PicoMLXServer](https://github.com/PicoMLX/PicoMLXServer)

- 🐍 [omlx](https://github.com/jundot/omlx) — LLM inference server with continuous batching & SSD caching, runs from macOS menu bar. ![](https://img.shields.io/github/stars/jundot/omlx?style=flat-square)
- 🐍 [lmstudio mlx-engine](https://github.com/lmstudio-ai/mlx-engine) — LM Studio's Apple MLX engine. ![](https://img.shields.io/github/stars/lmstudio-ai/mlx-engine?style=flat-square)
- 🐍 [mlx-omni-server](https://github.com/madroidmaq/mlx-omni-server) — Local inference server with OpenAI-compatible API for Apple Silicon. ![](https://img.shields.io/github/stars/madroidmaq/mlx-omni-server?style=flat-square)
- 🦅 [swama](https://github.com/Trans-N-ai/swama) — High-performance MLX inference engine for macOS with native Swift. ![](https://img.shields.io/github/stars/Trans-N-ai/swama?style=flat-square)
- 🐍 [mlx-llm](https://github.com/riccardomusmeci/mlx-llm) — LLM applications and tools running on Apple Silicon in real-time. ![](https://img.shields.io/github/stars/riccardomusmeci/mlx-llm?style=flat-square)
- 🐍 [fastmlx](https://github.com/arcee-ai/fastmlx) — High-performance production-ready API to host MLX models. ![](https://img.shields.io/github/stars/arcee-ai/fastmlx?style=flat-square)
- 🦅 [PicoMLXServer](https://github.com/PicoMLX/PicoMLXServer) — The easiest way to run MLX-based LLMs locally. ![](https://img.shields.io/github/stars/PicoMLX/PicoMLXServer?style=flat-square)
- 🐍 [mlx-openai-server](https://github.com/cubist38/mlx-openai-server) — OpenAI-compatible endpoints for MLX models. ![](https://img.shields.io/github/stars/cubist38/mlx-openai-server?style=flat-square)
- 🦅 [maclocal-api](https://github.com/scouzi1966/maclocal-api) — macOS server exposing Apple Foundation and MLX Models through unified OpenAI-compatible API. ![](https://img.shields.io/github/stars/scouzi1966/maclocal-api?style=flat-square)
- 🐍 [mlx_parallm](https://github.com/willccbb/mlx_parallm) — Fast parallel LLM inference for MLX. ![](https://img.shields.io/github/stars/willccbb/mlx_parallm?style=flat-square)
- 🐍 [mlx-gui](https://github.com/RamboRogers/mlx-gui) — MLX inference server with web UI for Apple Silicon. ![](https://img.shields.io/github/stars/RamboRogers/mlx-gui?style=flat-square)
- 🐍 [mlxserver](https://github.com/mustafaaljadery/mlxserver) — Simple inference server for the MLX library. ![](https://img.shields.io/github/stars/mustafaaljadery/mlxserver?style=flat-square)
- 🐍 [Toolio](https://github.com/OoriData/Toolio) — GenAI & agent toolkit for Apple Silicon, JSON schema-steered structured output and tool-calling. ![](https://img.shields.io/github/stars/OoriData/Toolio?style=flat-square)
- 🐍 [mlx_sharding](https://github.com/mzbac/mlx_sharding) — Distributed inference for MLX LLMs across multiple devices. ![](https://img.shields.io/github/stars/mzbac/mlx_sharding?style=flat-square)
- 🐍 [llamactl](https://github.com/lordmathis/llamactl) — Unified management and routing for llama.cpp, MLX and vLLM models. ![](https://img.shields.io/github/stars/lordmathis/llamactl?style=flat-square)
- 🐍 [Rapid-MLX](https://github.com/raullenchai/Rapid-MLX) — Fast local AI engine for Apple Silicon. 4.2x faster than Ollama, tool calling, prompt caching. OpenAI-compatible. ![](https://img.shields.io/github/stars/raullenchai/Rapid-MLX?style=flat-square)

## Training & Fine-tuning

- 🐍 [TransformerLab](https://github.com/transformerlab/transformerlab-app) — Open source research environment for training, evaluating, and scaling models. ![](https://img.shields.io/github/stars/transformerlab/transformerlab-app?style=flat-square)
- 🐍 [autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) — MLX port of Karpathy's autoresearch — autonomous AI research loops on Mac. ![](https://img.shields.io/github/stars/trevin-creator/autoresearch-mlx?style=flat-square)
- 🐍 [mlx-tune](https://github.com/ARahim3/mlx-tune) — Fine-tune LLMs on Mac: SFT, DPO, GRPO, Vision. Unsloth-compatible API. ![](https://img.shields.io/github/stars/ARahim3/mlx-tune?style=flat-square)
- 🐍 [mlx-lm-lora](https://github.com/Goekdeniz-Guelmez/mlx-lm-lora) — Train Large Language Models on MLX with LoRA. ![](https://img.shields.io/github/stars/Goekdeniz-Guelmez/mlx-lm-lora?style=flat-square)
- 🐍 [SiLLM](https://github.com/armbues/SiLLM) — Simplifies training and running LLMs on Apple Silicon via MLX. ![](https://img.shields.io/github/stars/armbues/SiLLM?style=flat-square)
- 🐍 [MLX-GRPO](https://github.com/Doriandarko/MLX-GRPO) — Pure MLX-based GRPO training pipeline on Apple Silicon. ![](https://img.shields.io/github/stars/Doriandarko/MLX-GRPO?style=flat-square)
- 🐍 [mamba.py](https://github.com/alxndrTL/mamba.py) — Simple and efficient Mamba (state-space model) in pure PyTorch and MLX. ![](https://img.shields.io/github/stars/alxndrTL/mamba.py?style=flat-square)
- 🐍 [mlx-snn](https://github.com/D-ST-Sword/mlx-snn) — Spiking Neural Network library built natively on MLX. ![](https://img.shields.io/github/stars/D-ST-Sword/mlx-snn?style=flat-square)
- 🐍 [mlx-gpt2](https://github.com/pranavjad/mlx-gpt2) — GPT-2 from scratch in MLX. Educational. ![](https://img.shields.io/github/stars/pranavjad/mlx-gpt2?style=flat-square)
- 🐍 [rlx](https://github.com/noahfarr/rlx) — Reinforcement learning framework based on MLX. ![](https://img.shields.io/github/stars/noahfarr/rlx?style=flat-square)
- 🐍 [Vodalus-Expert-LLM-Forge](https://github.com/severian42/Vodalus-Expert-LLM-Forge) — Dataset crafting with RAG + fine-tuning using MLX and Unsloth. ![](https://img.shields.io/github/stars/severian42/Vodalus-Expert-LLM-Forge?style=flat-square)
- 🐍 [unsloth-buddy](https://github.com/TYH-labs/unsloth-buddy) — Zero-friction LLM fine-tuning for agents; MLX on Apple Silicon. ![](https://img.shields.io/github/stars/TYH-labs/unsloth-buddy?style=flat-square)
- 🦀 [pmetal](https://github.com/Epistates/pmetal) — High performance LLM fine-tuning framework for Apple Silicon, written in Rust. ![](https://img.shields.io/github/stars/Epistates/pmetal?style=flat-square)

## Audio & Speech

- 🟨 [voicebox](https://github.com/jamiepine/voicebox) — The open-source voice synthesis studio. ![](https://img.shields.io/github/stars/jamiepine/voicebox?style=flat-square)
- 🐍 [mlx-audio](https://github.com/Blaizzy/mlx-audio) — TTS, STT and STS library built on MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-audio?style=flat-square)
- 🐍 [lightning-whisper-mlx](https://github.com/mustafaaljadery/lightning-whisper-mlx) — Extremely fast Whisper optimized for Apple Silicon. ![](https://img.shields.io/github/stars/mustafaaljadery/lightning-whisper-mlx?style=flat-square)
- 🐍 [parakeet-mlx](https://github.com/senstella/parakeet-mlx) — Nvidia's Parakeet models for Apple Silicon. ![](https://img.shields.io/github/stars/senstella/parakeet-mlx?style=flat-square)
- 🐍 [TheWhisper](https://github.com/TheStageAI/TheWhisper) — Optimized Whisper for streaming and on-device use. ![](https://img.shields.io/github/stars/TheStageAI/TheWhisper?style=flat-square)
- 🐍 [f5-tts-mlx](https://github.com/lucasnewman/f5-tts-mlx) — F5-TTS in MLX. ![](https://img.shields.io/github/stars/lucasnewman/f5-tts-mlx?style=flat-square)
- 🐍 [Lightning-SimulWhisper](https://github.com/altalt-org/Lightning-SimulWhisper) — MLX/CoreML streaming Whisper, ~15x faster. ![](https://img.shields.io/github/stars/altalt-org/Lightning-SimulWhisper?style=flat-square)
- 🦅 [speech-swift](https://github.com/soniqo/speech-swift) — AI speech toolkit — ASR, TTS, speech-to-speech, VAD, diarization. ![](https://img.shields.io/github/stars/soniqo/speech-swift?style=flat-square)
- 🦅 [mlx-audio-swift](https://github.com/Blaizzy/mlx-audio-swift) — Modular Swift SDK for audio processing with MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-audio-swift?style=flat-square)
- 🐍 [qwen3-tts-apple-silicon](https://github.com/kapi2800/qwen3-tts-apple-silicon) — Qwen3-TTS on Mac. Voice cloning, 100% offline. ![](https://img.shields.io/github/stars/kapi2800/qwen3-tts-apple-silicon?style=flat-square)
- 🐍 [csm-mlx](https://github.com/senstella/csm-mlx) — Conversation Speech Model for Apple Silicon. ![](https://img.shields.io/github/stars/senstella/csm-mlx?style=flat-square)
- 🐍 [MLX-Auto-Subtitled-Video-Generator](https://github.com/RayFernando1337/MLX-Auto-Subtitled-Video-Generator) — Generate accurate video transcripts using MLX. ![](https://img.shields.io/github/stars/RayFernando1337/MLX-Auto-Subtitled-Video-Generator?style=flat-square)
- 🐍 [wtm](https://github.com/JosefAlbers/wtm) — Blazing fast Whisper Turbo for speech-to-text on Mac. ![](https://img.shields.io/github/stars/JosefAlbers/wtm?style=flat-square)
- 🦅 [kokoro-ios](https://github.com/mlalma/kokoro-ios) — Kokoro TTS for iOS and macOS via MLX. ![](https://img.shields.io/github/stars/mlalma/kokoro-ios?style=flat-square)
- 🐍 [whisply](https://github.com/tsmdt/whisply) — Fast CLI/GUI for batch transcription and translation. ![](https://img.shields.io/github/stars/tsmdt/whisply?style=flat-square)
- 🐍 [nanospeech](https://github.com/lucasnewman/nanospeech) — Simple, hackable TTS in PyTorch and MLX. ![](https://img.shields.io/github/stars/lucasnewman/nanospeech?style=flat-square)

## Image & Video Generation

- 🐍 [mflux](https://github.com/filipstrand/mflux) — MLX native Flux and Stable Diffusion image generation. ![](https://img.shields.io/github/stars/filipstrand/mflux?style=flat-square)
- 🐍 [mlx-video](https://github.com/Blaizzy/mlx-video) — Image-Video-Audio generation models on Mac. ![](https://img.shields.io/github/stars/Blaizzy/mlx-video?style=flat-square)
- 🦅 [flux.swift](https://github.com/mzbac/flux.swift) — Swift implementation of Flux.1 using mlx-swift. ![](https://img.shields.io/github/stars/mzbac/flux.swift?style=flat-square)
- 🐍 [mlxstudio](https://github.com/jjang-ai/mlxstudio) — MLX Studio — Image Gen/Edit + Chat/Code all in one. ![](https://img.shields.io/github/stars/jjang-ai/mlxstudio?style=flat-square)
- 🐍 [MFLUX-WEBUI](https://github.com/CharafChnioune/MFLUX-WEBUI) — Web UI for MFLUX image generation using MLX and FLUX models. ![](https://img.shields.io/github/stars/CharafChnioune/MFLUX-WEBUI?style=flat-square)
- 🦅 [flux-generator](https://github.com/voipnuggets/flux-generator) — Local image and music generation for Apple Silicon. ![](https://img.shields.io/github/stars/voipnuggets/flux-generator?style=flat-square)

## Vision & Multimodal

- 🐍 [mlx-vlm](https://github.com/Blaizzy/mlx-vlm) — Vision Language Models on Mac using MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-vlm?style=flat-square)
- 🐍 [ml-aim](https://github.com/apple/ml-aim) — Apple's AIMv1 and AIMv2 vision models. ![](https://img.shields.io/github/stars/apple/ml-aim?style=flat-square)
- 🐍 [pvm](https://github.com/JosefAlbers/pvm) — Phi-3.5 Vision and Language Models for Mac. ![](https://img.shields.io/github/stars/JosefAlbers/pvm?style=flat-square)
- 🐍 [photo-similarity-search](https://github.com/harperreed/photo-similarity-search) — CLIP-based photo similarity for Apple Silicon. ![](https://img.shields.io/github/stars/harperreed/photo-similarity-search?style=flat-square)

## Embeddings & RAG

- 🐍 [mlx-embeddings](https://github.com/Blaizzy/mlx-embeddings) — Vision and Language Embedding models locally on Mac. ![](https://img.shields.io/github/stars/Blaizzy/mlx-embeddings?style=flat-square)
- 🦅 [VecturaKit](https://github.com/rryam/VecturaKit) — Swift vector database for on-device RAG. ![](https://img.shields.io/github/stars/rryam/VecturaKit?style=flat-square)
- 🐍 [jina-grep-cli](https://github.com/jina-ai/jina-grep-cli) — Semantic grep powered by Jina embeddings (MLX). ![](https://img.shields.io/github/stars/jina-ai/jina-grep-cli?style=flat-square)
- 🐍 [sisi](https://github.com/frost-beta/sisi) — Semantic image search CLI using MLX embeddings. ![](https://img.shields.io/github/stars/frost-beta/sisi?style=flat-square)
- 🐍 [mlx-retrieval](https://github.com/jina-ai/mlx-retrieval) — Train embedding and reranker models on Apple Silicon. ![](https://img.shields.io/github/stars/jina-ai/mlx-retrieval?style=flat-square)
- 🐍 [mlx-rag](https://github.com/vegaluisjose/mlx-rag) — Simple RAG application running locally on Apple Silicon. ![](https://img.shields.io/github/stars/vegaluisjose/mlx-rag?style=flat-square)
- 🐍 [mlx_clip](https://github.com/harperreed/mlx_clip) — CLIP on Apple Silicon using MLX. ![](https://img.shields.io/github/stars/harperreed/mlx_clip?style=flat-square)

## Swift Ecosystem

Native macOS/iOS apps and packages built on MLX. See also: [mlx-swift](https://github.com/ml-explore/mlx-swift) in Core, [swama](https://github.com/Trans-N-ai/swama) in Inference, [mlx-audio-swift](https://github.com/Blaizzy/mlx-audio-swift) in Audio. Getting started? Read [On-device ML research with MLX and Swift](https://www.swift.org/blog/mlx-swift/).

- 🦅 [osaurus](https://github.com/osaurus-ai/osaurus) — Native macOS AI agent — any model, persistent memory, autonomous execution. ![](https://img.shields.io/github/stars/osaurus-ai/osaurus?style=flat-square)
- 🦅 [Klee](https://github.com/signerlabs/Klee) — Native macOS AI chat, 100% local inference. ![](https://img.shields.io/github/stars/signerlabs/Klee?style=flat-square)
- 🦅 [ChatMLX](https://github.com/johnmai-dev/ChatMLX) — High-performance chat app for macOS. ![](https://img.shields.io/github/stars/johnmai-dev/ChatMLX?style=flat-square)
- 🦅 [Fabric](https://github.com/Fabric-Project/Fabric) — Creative Coding / 3D / Image Processing, inspired by Quartz Composer. ![](https://img.shields.io/github/stars/Fabric-Project/Fabric?style=flat-square)
- 🦅 [mlx-swift-chat](https://github.com/preternatural-explore/mlx-swift-chat) — Multi-platform SwiftUI frontend for local LLMs. ![](https://img.shields.io/github/stars/preternatural-explore/mlx-swift-chat?style=flat-square)
- 🦅 [fullmoon-ios](https://github.com/mainframecomputer/fullmoon-ios) — Chat with local LLMs on iPhone, iPad, Mac. ![](https://img.shields.io/github/stars/mainframecomputer/fullmoon-ios?style=flat-square)
- 🦅 [LocalLLMClient](https://github.com/tattn/LocalLLMClient) — Swift package for local LLMs on iOS, macOS, Linux. ![](https://img.shields.io/github/stars/tattn/LocalLLMClient?style=flat-square)
- 🦅 [MLX-Outil](https://github.com/rudrankriyam/MLX-Outil) — Tool calling using MLX Swift across iOS, macOS, and visionOS. ![](https://img.shields.io/github/stars/rudrankriyam/MLX-Outil?style=flat-square)
- 🦅 [mlx-swift-audio](https://github.com/DePasqualeOrg/mlx-swift-audio) — Swift tools for TTS and STT powered by MLX. ![](https://img.shields.io/github/stars/DePasqualeOrg/mlx-swift-audio?style=flat-square)
- 🦅 [f5-tts-swift](https://github.com/lucasnewman/f5-tts-swift) — F5-TTS implementation in Swift using MLX. ![](https://img.shields.io/github/stars/lucasnewman/f5-tts-swift?style=flat-square)

## Benchmarks

- 🦅 [Metal-Puzzles](https://github.com/abeleinin/Metal-Puzzles) — Solve puzzles. Learn Metal GPU programming. ![](https://img.shields.io/github/stars/abeleinin/Metal-Puzzles?style=flat-square)
- 🐍 [mlx-benchmark](https://github.com/TristanBilot/mlx-benchmark) — Benchmark MLX ops on all Apple Silicon chips (GPU, CPU) + MPS and CUDA. ![](https://img.shields.io/github/stars/TristanBilot/mlx-benchmark?style=flat-square)
- 🐍 [mlx-bitnet](https://github.com/exo-explore/mlx-bitnet) — 1.58 Bit LLM on Apple Silicon. ![](https://img.shields.io/github/stars/exo-explore/mlx-bitnet?style=flat-square)

## Apps & Demos

- 🐍 [chat-with-mlx](https://github.com/qnguyen3/chat-with-mlx) — All-in-one LLMs Chat UI for Apple Silicon. ![](https://img.shields.io/github/stars/qnguyen3/chat-with-mlx?style=flat-square)
- 🐍 [cross-market-state-fusion](https://github.com/humanplane/cross-market-state-fusion) — RL agent fusing Binance futures into Polymarket. On-device training with MLX. ![](https://img.shields.io/github/stars/humanplane/cross-market-state-fusion?style=flat-square)
- 🦅 [NotebookMLX](https://github.com/johnmai-dev/NotebookMLX) — Open source NotebookLM. ![](https://img.shields.io/github/stars/johnmai-dev/NotebookMLX?style=flat-square)
- 🟨 [nodetool](https://github.com/nodetool-ai/nodetool) — Visual builder for AI Workflows and Agents. ![](https://img.shields.io/github/stars/nodetool-ai/nodetool?style=flat-square)
- 🐍 [Vim-LM](https://github.com/JosefAlbers/Vim-LM) — AI Copilot for Vim/NeoVim. ![](https://img.shields.io/github/stars/JosefAlbers/Vim-LM?style=flat-square)
- 🐍 [mlx-ui](https://github.com/da-z/mlx-ui) — Simple web UI for MLX using Streamlit. ![](https://img.shields.io/github/stars/da-z/mlx-ui?style=flat-square)
- 🟨 [Silicon-Studio](https://github.com/rileycleavenger/Silicon-Studio) — Fine-tune and run LLMs locally on M-series Mac. ![](https://img.shields.io/github/stars/rileycleavenger/Silicon-Studio?style=flat-square)
- 🐍 [llm-mlx](https://github.com/simonw/llm-mlx) — MLX model support plugin for Simon Willison's LLM tool. ![](https://img.shields.io/github/stars/simonw/llm-mlx?style=flat-square)
- 🐍 [mlx-chat-app](https://github.com/mlx-chat/mlx-chat-app) — macOS chat app connecting local docs to MLX-powered LLMs. ![](https://img.shields.io/github/stars/mlx-chat/mlx-chat-app?style=flat-square)
- 🐍 [jarvis-mlx](https://github.com/huwprosser/jarvis-mlx) — All-in-one offline productivity assistant using MLX. ![](https://img.shields.io/github/stars/huwprosser/jarvis-mlx?style=flat-square)
- 🦅 [AirPosture](https://github.com/allenv0/AirPosture) — AirPods as AI posture coach on iOS, powered by MLX. ![](https://img.shields.io/github/stars/allenv0/AirPosture?style=flat-square)
- 🐍 [nanoGPT_mlx](https://github.com/vithursant/nanoGPT_mlx) — Karpathy's nanoGPT on Apple MLX. ![](https://img.shields.io/github/stars/vithursant/nanoGPT_mlx?style=flat-square)
- 🐍 [m-courtyard](https://github.com/Mcourtyard/m-courtyard) — Local AI model fine-tuning assistant, zero-code. ![](https://img.shields.io/github/stars/Mcourtyard/m-courtyard?style=flat-square)

## Other Tools

- 🦀 [llmfit](https://github.com/AlexsJones/llmfit) — One command to find what LLM runs on your hardware. ![](https://img.shields.io/github/stars/AlexsJones/llmfit?style=flat-square)
- 🐍 [einops](https://github.com/arogozhnikov/einops) — Flexible tensor operations (supports MLX). ![](https://img.shields.io/github/stars/arogozhnikov/einops?style=flat-square)
- 🐍 [outlinesmlx](https://github.com/sacha-ichbiah/outlines-mlx) — Guided generation on Apple Silicon using Outlines + MLX. ![](https://img.shields.io/github/stars/sacha-ichbiah/outlines-mlx?style=flat-square)
- 🐍 [olla](https://github.com/thushan/olla) — Lightweight proxy/load balancer for LLM infra (llama.cpp, MLX, vLLM). ![](https://img.shields.io/github/stars/thushan/olla?style=flat-square)
- 🐍 [anubis-oss](https://github.com/uncSoft/anubis-oss) — Local LLM testing and benchmarking for Apple Silicon. ![](https://img.shields.io/github/stars/uncSoft/anubis-oss?style=flat-square)

## Models

**Where to find models:**
- [mlx-community on HuggingFace](https://huggingface.co/mlx-community) — 2000+ MLX-optimized models ready to use
- [lmstudio-community on HuggingFace](https://huggingface.co/lmstudio-community) — LM Studio's curated MLX models
- [Using MLX at Hugging Face](https://huggingface.co/docs/hub/en/mlx) — Official HuggingFace MLX docs

**Which model for my Mac?**

| RAM | Recommended models | Notes |
|-----|-------------------|-------|
| 8GB | Qwen3.5-4B-4bit, Phi-4-mini-4bit | Small but capable |
| 16GB | Qwen3.5-9B-4bit, Gemma-3-12B-4bit | Great balance |
| 32GB | Qwen3.5-27B-4bit, Devstral-24B-4bit | Strong coding + reasoning |
| 64GB+ | Qwen3.5-122B-A10B-4bit, Llama-4-Scout | Near-frontier quality |

## Learning Resources

- [On-device ML research with MLX and Swift](https://www.swift.org/blog/mlx-swift/) — Official Swift blog (2024)
- [Deep Dive into AI with MLX and PyTorch](https://github.com/neobundy/Deep-Dive-Into-AI-With-MLX-PyTorch) — Comprehensive educational resource
- [Deploying LLMs locally with MLX](https://towardsdatascience.com/deploying-llms-locally-with-apples-mlx-framework-2b3862049a93) — Toward Data Science
- [MLX Community Projects](https://github.com/ml-explore/mlx/discussions/654) — Official MLX discussion thread for community projects

---

## Contributing

Built something with MLX? We want to list it!

**Easiest way:** [Open an issue](https://github.com/raullenchai/awesome-mlx/issues/new?template=submit_project.yml) with your project name, URL, and a one-line description. We'll add it for you.

**PR way:** Add your project to the right category using this format:
```
- 🐍 [name](url) — One-line description. ![](https://img.shields.io/github/stars/OWNER/REPO?style=flat-square)
```

**Add a badge to your README** (optional):
```markdown
[![Awesome MLX](https://img.shields.io/badge/Awesome-MLX-blue?style=flat-square)](https://github.com/raullenchai/awesome-mlx)
```

Guidelines:
- Language emoji: 🐍 Python · 🦅 Swift · 🟨 JS/TS · 🦀 Rust · 🐹 Go
- Sort entries by stars (descending) within each section
- All MLX projects welcome — no minimum star count

## License

[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
