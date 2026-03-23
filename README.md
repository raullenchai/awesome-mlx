# Awesome MLX [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome projects, tools, models, and resources for [Apple MLX](https://github.com/ml-explore/mlx) — the ML framework for Apple Silicon.

MLX is designed for efficient and flexible machine learning on Apple silicon. This list tracks the best of the growing MLX ecosystem — from inference engines to training tools, audio to vision, Swift apps to benchmarks.

**Contributing:** PRs welcome! Please keep entries sorted by stars (descending) within each section.

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
- [Articles & Tutorials](#articles--tutorials)
- [Models](#models)

---

## Core Framework

- [mlx](https://github.com/ml-explore/mlx) — Apple's array framework for ML on Apple silicon. The foundation. ![](https://img.shields.io/github/stars/ml-explore/mlx?style=flat-square)
- [mlx-examples](https://github.com/ml-explore/mlx-examples) — Official examples: LLMs, LoRA, Stable Diffusion, Whisper, and more. ![](https://img.shields.io/github/stars/ml-explore/mlx-examples?style=flat-square)
- [mlx-lm](https://github.com/ml-explore/mlx-lm) — Apple's official "run LLMs with MLX" package. Text generation, quantization, LoRA. ![](https://img.shields.io/github/stars/ml-explore/mlx-lm?style=flat-square)
- [mlx-swift](https://github.com/ml-explore/mlx-swift) — Swift API for MLX. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift?style=flat-square)
- [mlx-swift-examples](https://github.com/ml-explore/mlx-swift-examples) — Examples using MLX Swift: LLMs, image generation, training. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift-examples?style=flat-square)
- [mlx-swift-lm](https://github.com/ml-explore/mlx-swift-lm) — LLMs and VLMs with MLX Swift. ![](https://img.shields.io/github/stars/ml-explore/mlx-swift-lm?style=flat-square)
- [node-mlx](https://github.com/frost-beta/node-mlx) — Machine learning framework for Node.js, built on MLX. ![](https://img.shields.io/github/stars/frost-beta/node-mlx?style=flat-square)
- [mlx-graphs](https://github.com/mlx-graphs/mlx-graphs) — Graph Neural Network library for Apple Silicon. ![](https://img.shields.io/github/stars/mlx-graphs/mlx-graphs?style=flat-square)

## Inference & Serving

- [Rapid-MLX](https://github.com/raullenchai/Rapid-MLX) — The fastest local AI engine for Apple Silicon. 4.2x faster than Ollama, 100% tool calling, prompt caching. Drop-in OpenAI replacement. ![](https://img.shields.io/github/stars/raullenchai/Rapid-MLX?style=flat-square)
- [omlx](https://github.com/jundot/omlx) — LLM inference server with continuous batching & SSD caching, runs from the macOS menu bar. ![](https://img.shields.io/github/stars/jundot/omlx?style=flat-square)
- [lmstudio mlx-engine](https://github.com/lmstudio-ai/mlx-engine) — LM Studio's Apple MLX engine. ![](https://img.shields.io/github/stars/lmstudio-ai/mlx-engine?style=flat-square)
- [mlx-omni-server](https://github.com/madroidmaq/mlx-omni-server) — Local inference server with OpenAI-compatible API for Apple Silicon. ![](https://img.shields.io/github/stars/madroidmaq/mlx-omni-server?style=flat-square)
- [vllm-mlx](https://github.com/waybarrios/vllm-mlx) — OpenAI/Anthropic-compatible server. Continuous batching, MCP tool calling, multimodal. ![](https://img.shields.io/github/stars/waybarrios/vllm-mlx?style=flat-square)
- [swama](https://github.com/Trans-N-ai/swama) — High-performance MLX-based LLM inference engine for macOS with native Swift. ![](https://img.shields.io/github/stars/Trans-N-ai/swama?style=flat-square)
- [mlx-llm](https://github.com/riccardomusmeci/mlx-llm) — LLM applications and tools running on Apple Silicon in real-time. ![](https://img.shields.io/github/stars/riccardomusmeci/mlx-llm?style=flat-square)
- [fastmlx](https://github.com/arcee-ai/fastmlx) — High-performance production-ready API to host MLX models. ![](https://img.shields.io/github/stars/arcee-ai/fastmlx?style=flat-square)
- [PicoMLXServer](https://github.com/PicoMLX/PicoMLXServer) — The easiest way to run the fastest MLX-based LLMs locally. ![](https://img.shields.io/github/stars/PicoMLX/PicoMLXServer?style=flat-square)
- [mlx-openai-server](https://github.com/cubist38/mlx-openai-server) — High-performance API server providing OpenAI-compatible endpoints for MLX models. ![](https://img.shields.io/github/stars/cubist38/mlx-openai-server?style=flat-square)
- [maclocal-api](https://github.com/scouzi1966/maclocal-api) — macOS server exposing Apple Foundation and MLX Models through unified OpenAI-compatible API. ![](https://img.shields.io/github/stars/scouzi1966/maclocal-api?style=flat-square)
- [Toolio](https://github.com/OoriData/Toolio) — GenAI & agent toolkit for Apple Silicon Mac, JSON schema-steered structured output and tool-calling. ![](https://img.shields.io/github/stars/OoriData/Toolio?style=flat-square)

## Training & Fine-tuning

- [TransformerLab](https://github.com/transformerlab/transformerlab-app) — Open source research environment for training, evaluating, and scaling models. ![](https://img.shields.io/github/stars/transformerlab/transformerlab-app?style=flat-square)
- [autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) — Apple Silicon (MLX) port of Karpathy's autoresearch — autonomous AI research loops on Mac. ![](https://img.shields.io/github/stars/trevin-creator/autoresearch-mlx?style=flat-square)
- [mlx-tune](https://github.com/ARahim3/mlx-tune) — Fine-tune LLMs on Mac: SFT, DPO, GRPO, Vision fine-tuning natively on MLX. Unsloth-compatible API. ![](https://img.shields.io/github/stars/ARahim3/mlx-tune?style=flat-square)
- [mlx-lm-lora](https://github.com/Goekdeniz-Guelmez/mlx-lm-lora) — Train Large Language Models on MLX with LoRA. ![](https://img.shields.io/github/stars/Goekdeniz-Guelmez/mlx-lm-lora?style=flat-square)
- [SiLLM](https://github.com/armbues/SiLLM) — Simplifies training and running LLMs on Apple Silicon via MLX. ![](https://img.shields.io/github/stars/armbues/SiLLM?style=flat-square)
- [MLX-GRPO](https://github.com/Doriandarko/MLX-GRPO) — Pure MLX-based training pipeline for fine-tuning LLMs using GRPO on Apple Silicon. ![](https://img.shields.io/github/stars/Doriandarko/MLX-GRPO?style=flat-square)
- [pmetal](https://github.com/Epistates/pmetal) — Powdered Metal — High performance LLM fine-tuning framework for Apple Silicon, written in Rust. ![](https://img.shields.io/github/stars/Epistates/pmetal?style=flat-square)

## Audio & Speech

- [voicebox](https://github.com/jamiepine/voicebox) — The open-source voice synthesis studio. ![](https://img.shields.io/github/stars/jamiepine/voicebox?style=flat-square)
- [mlx-audio](https://github.com/Blaizzy/mlx-audio) — TTS, STT and STS library built on MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-audio?style=flat-square)
- [lightning-whisper-mlx](https://github.com/mustafaaljadery/lightning-whisper-mlx) — Extremely fast Whisper implementation optimized for Apple Silicon. ![](https://img.shields.io/github/stars/mustafaaljadery/lightning-whisper-mlx?style=flat-square)
- [parakeet-mlx](https://github.com/senstella/parakeet-mlx) — Nvidia's Parakeet models for Apple Silicon using MLX. ![](https://img.shields.io/github/stars/senstella/parakeet-mlx?style=flat-square)
- [TheWhisper](https://github.com/TheStageAI/TheWhisper) — Optimized Whisper models for streaming and on-device use. ![](https://img.shields.io/github/stars/TheStageAI/TheWhisper?style=flat-square)
- [f5-tts-mlx](https://github.com/lucasnewman/f5-tts-mlx) — Implementation of F5-TTS in MLX. ![](https://img.shields.io/github/stars/lucasnewman/f5-tts-mlx?style=flat-square)
- [Lightning-SimulWhisper](https://github.com/altalt-org/Lightning-SimulWhisper) — MLX/CoreML streaming Whisper with ~15x performance increase. ![](https://img.shields.io/github/stars/altalt-org/Lightning-SimulWhisper?style=flat-square)
- [speech-swift](https://github.com/soniqo/speech-swift) — AI speech toolkit for Apple Silicon — ASR, TTS, speech-to-speech, VAD, diarization. ![](https://img.shields.io/github/stars/soniqo/speech-swift?style=flat-square)
- [mlx-audio-swift](https://github.com/Blaizzy/mlx-audio-swift) — Modular Swift SDK for audio processing with MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-audio-swift?style=flat-square)
- [qwen3-tts-apple-silicon](https://github.com/kapi2800/qwen3-tts-apple-silicon) — Run Qwen3-TTS locally on Mac. Voice cloning, custom voices, 100% offline. ![](https://img.shields.io/github/stars/kapi2800/qwen3-tts-apple-silicon?style=flat-square)
- [csm-mlx](https://github.com/senstella/csm-mlx) — Conversation Speech Model implementation for Apple Silicon using MLX. ![](https://img.shields.io/github/stars/senstella/csm-mlx?style=flat-square)
- [nanospeech](https://github.com/lucasnewman/nanospeech) — Simple, hackable text-to-speech in PyTorch and MLX. ![](https://img.shields.io/github/stars/lucasnewman/nanospeech?style=flat-square)

## Image & Video Generation

- [mflux](https://github.com/filipstrand/mflux) — MLX native Flux and Stable Diffusion image generation. ![](https://img.shields.io/github/stars/filipstrand/mflux?style=flat-square)
- [mlx-video](https://github.com/Blaizzy/mlx-video) — Inference and finetuning of Image-Video-Audio generation models on Mac. ![](https://img.shields.io/github/stars/Blaizzy/mlx-video?style=flat-square)
- [flux.swift](https://github.com/mzbac/flux.swift) — Swift implementation of Flux.1 using mlx-swift. ![](https://img.shields.io/github/stars/mzbac/flux.swift?style=flat-square)
- [mlxstudio](https://github.com/jjang-ai/mlxstudio) — MLX Studio — Image Gen/Edit + Chat/Code all in one. ![](https://img.shields.io/github/stars/jjang-ai/mlxstudio?style=flat-square)

## Vision & Multimodal

- [mlx-vlm](https://github.com/Blaizzy/mlx-vlm) — Inference and fine-tuning of Vision Language Models on Mac using MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-vlm?style=flat-square)
- [ml-aim](https://github.com/apple/ml-aim) — Apple's AIMv1 and AIMv2 vision models. ![](https://img.shields.io/github/stars/apple/ml-aim?style=flat-square)
- [photo-similarity-search](https://github.com/harperreed/photo-similarity-search) — CLIP-based photo similarity web app for Apple Silicon. ![](https://img.shields.io/github/stars/harperreed/photo-similarity-search?style=flat-square)

## Embeddings & RAG

- [mlx-embeddings](https://github.com/Blaizzy/mlx-embeddings) — Running Vision and Language Embedding models locally on Mac using MLX. ![](https://img.shields.io/github/stars/Blaizzy/mlx-embeddings?style=flat-square)
- [VecturaKit](https://github.com/rryam/VecturaKit) — Swift-based vector database for on-device RAG using MLTensor and MLX Embedders. ![](https://img.shields.io/github/stars/rryam/VecturaKit?style=flat-square)
- [jina-grep-cli](https://github.com/jina-ai/jina-grep-cli) — Semantic grep powered by Jina embeddings v5 (MLX on Apple Silicon). ![](https://img.shields.io/github/stars/jina-ai/jina-grep-cli?style=flat-square)
- [mlx-retrieval](https://github.com/jina-ai/mlx-retrieval) — Train embedding and reranker models for retrieval tasks on Apple Silicon. ![](https://img.shields.io/github/stars/jina-ai/mlx-retrieval?style=flat-square)

## Swift Ecosystem

Native macOS/iOS apps built on MLX.

- [osaurus](https://github.com/osaurus-ai/osaurus) — Native macOS AI agent harness — any model, persistent memory, autonomous execution. ![](https://img.shields.io/github/stars/osaurus-ai/osaurus?style=flat-square)
- [Klee](https://github.com/signerlabs/Klee) — Native macOS AI chat app powered by MLX. 100% local inference. ![](https://img.shields.io/github/stars/signerlabs/Klee?style=flat-square)
- [ChatMLX](https://github.com/johnmai-dev/ChatMLX) — Modern, open-source, high-performance chat app for macOS based on LLMs. ![](https://img.shields.io/github/stars/johnmai-dev/ChatMLX?style=flat-square)
- [Fabric](https://github.com/Fabric-Project/Fabric) — Node Creative Coding / 3D / Image Processing tool inspired by Quartz Composer. ![](https://img.shields.io/github/stars/Fabric-Project/Fabric?style=flat-square)
- [mlx-swift-chat](https://github.com/preternatural-explore/mlx-swift-chat) — Multi-platform SwiftUI frontend for running local LLMs with MLX. ![](https://img.shields.io/github/stars/preternatural-explore/mlx-swift-chat?style=flat-square)
- [fullmoon-ios](https://github.com/mainframecomputer/fullmoon-ios) — Chat with local LLMs optimized for Apple Silicon — iPhone, iPad, Mac. ![](https://img.shields.io/github/stars/mainframecomputer/fullmoon-ios?style=flat-square)
- [LocalLLMClient](https://github.com/tattn/LocalLLMClient) — Swift package to run local LLMs on iOS, macOS, Linux. ![](https://img.shields.io/github/stars/tattn/LocalLLMClient?style=flat-square)

## Benchmarks

- [Metal-Puzzles](https://github.com/abeleinin/Metal-Puzzles) — Solve puzzles. Learn Metal GPU programming. ![](https://img.shields.io/github/stars/abeleinin/Metal-Puzzles?style=flat-square)
- [mlx-benchmark](https://github.com/TristanBilot/mlx-benchmark) — Benchmark of MLX operations on all Apple Silicon chips (GPU, CPU) + MPS and CUDA. ![](https://img.shields.io/github/stars/TristanBilot/mlx-benchmark?style=flat-square)
- [mlx-bitnet](https://github.com/exo-explore/mlx-bitnet) — 1.58 Bit LLM on Apple Silicon using MLX. ![](https://img.shields.io/github/stars/exo-explore/mlx-bitnet?style=flat-square)

## Apps & Demos

- [chat-with-mlx](https://github.com/qnguyen3/chat-with-mlx) — All-in-one LLMs Chat UI for Apple Silicon Mac using MLX. ![](https://img.shields.io/github/stars/qnguyen3/chat-with-mlx?style=flat-square)
- [cross-market-state-fusion](https://github.com/humanplane/cross-market-state-fusion) — RL agent fusing real-time Binance futures data into Polymarket. On-device training with MLX. ![](https://img.shields.io/github/stars/humanplane/cross-market-state-fusion?style=flat-square)
- [NotebookMLX](https://github.com/johnmai-dev/NotebookMLX) — Open source version of NotebookLM. ![](https://img.shields.io/github/stars/johnmai-dev/NotebookMLX?style=flat-square)
- [nodetool](https://github.com/nodetool-ai/nodetool) — Visual builder for AI Workflows and Agents. ![](https://img.shields.io/github/stars/nodetool-ai/nodetool?style=flat-square)
- [Vim-LM](https://github.com/JosefAlbers/Vim-LM) — AI Copilot for Vim/NeoVim. ![](https://img.shields.io/github/stars/JosefAlbers/Vim-LM?style=flat-square)
- [mlx-ui](https://github.com/da-z/mlx-ui) — Simple UI / Web / Frontend for MLX using Streamlit. ![](https://img.shields.io/github/stars/da-z/mlx-ui?style=flat-square)
- [Silicon-Studio](https://github.com/rileycleavenger/Silicon-Studio) — Fine-tune and run LLMs locally on M-series Mac. ![](https://img.shields.io/github/stars/rileycleavenger/Silicon-Studio?style=flat-square)
- [nanoGPT_mlx](https://github.com/vithursant/nanoGPT_mlx) — Port of Karpathy's nanoGPT to Apple MLX. ![](https://img.shields.io/github/stars/vithursant/nanoGPT_mlx?style=flat-square)

## Other Tools

- [llmfit](https://github.com/AlexsJones/llmfit) — Hundreds of models & providers. One command to find what runs on your hardware. ![](https://img.shields.io/github/stars/AlexsJones/llmfit?style=flat-square)
- [einops](https://github.com/arogozhnikov/einops) — Flexible and powerful tensor operations for readable and reliable code (supports MLX). ![](https://img.shields.io/github/stars/arogozhnikov/einops?style=flat-square)
- [outlinesmlx](https://github.com/sacha-ichbiah/outlines-mlx) — Fast minimalistic guided generation on Apple Silicon using Outlines and MLX. ![](https://img.shields.io/github/stars/sacha-ichbiah/outlines-mlx?style=flat-square)

## Articles & Tutorials

### 2026
- [Autoresearch on MLX](https://github.com/trevin-creator/autoresearch-mlx) — Running autonomous AI experiments on Apple Silicon
- [Fine-tuning LLMs on Apple Silicon with mlx-tune](https://github.com/ARahim3/mlx-tune) — SFT, DPO, GRPO natively on MLX

### 2025
- [MLX Distributed: Scaling inference across Apple Silicon](https://github.com/exo-explore/exo) — Distributed inference with tensor parallelism + RDMA over Thunderbolt 5

### 2024
- [On-device ML research with MLX and Swift](https://www.swift.org/blog/mlx-swift/) — Official Swift blog
- [MLX: On-device machine learning on Apple Silicon](https://antran.app/2024/mlx_getting_started/) — Getting started guide
- [Deploying LLMs locally with Apple's MLX framework](https://towardsdatascience.com/deploying-llms-locally-with-apples-mlx-framework-2b3862049a93) — Toward Data Science
- [Deep Dive into AI with MLX and PyTorch](https://github.com/neobundy/Deep-Dive-Into-AI-With-MLX-PyTorch) — Comprehensive educational resource

## Models

- [mlx-community on HuggingFace](https://huggingface.co/mlx-community) — 2000+ MLX-optimized models ready to use
- [Using MLX at Hugging Face](https://huggingface.co/docs/hub/en/mlx) — Official HuggingFace MLX docs
- [lmstudio-community on HuggingFace](https://huggingface.co/lmstudio-community) — LM Studio's curated MLX models

---

## Contributing

Contributions welcome! Please:
1. Keep entries sorted by stars (descending) within each section
2. Include a brief description (one line)
3. Only add projects with 50+ stars or notable technical merit
4. Use the format: `- [name](url) — Description. ![stars badge]`

## License

[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
