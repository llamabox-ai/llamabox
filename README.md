# LlamaBox

**Offline AI chat for Android — run large language models locally on your phone with zero internet required.**

[![License: AGPL--3.0](https://img.shields.io/badge/license-AGPL--3.0-blue)](LICENSE)
![Platform: Android 7.0+](https://img.shields.io/badge/platform-Android--7.0%2B-green)
![Built with: React Native](https://img.shields.io/badge/built%20with-React%20Native-61DAFB)
![Status: closed beta](https://img.shields.io/badge/status-closed%20beta-orange)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](CONTRIBUTING.md)

LlamaBox is a private, fully offline AI chat app for Android that lets you download and run quantized GGUF models directly on your device. No cloud servers, no user accounts, and no data collection — your conversations stay on your phone, making it the ideal private ChatGPT alternative for anyone who values confidentiality. Whether you want a local LLM for brainstorming, coding help, or an offline AI assistant while traveling, LlamaBox delivers on-device intelligence without an internet connection.

## Screenshots

![LlamaBox home screen with offline AI chat model management on Android](https://llamabox-ai.github.io/assets/screenshot-1-home.png)
![Local LLM chat interface running a private AI conversation on Android](https://llamabox-ai.github.io/assets/screenshot-3-chat.png)
![LlamaBox model sidebar for managing downloaded GGUF models](https://llamabox-ai.github.io/assets/screenshot-sidebar.png)
![Settings screen for the offline AI assistant app](https://llamabox-ai.github.io/assets/screenshot-settings.png)

## Features

- **Fully Offline** — Download your favorite quantized models once, then chat anywhere without Wi-Fi or mobile data.
- **Multimodal Vision** — Chat with images using on-device LLaVA-style models; point your camera and ask questions completely offline.
- **Voice Output** — Listen to AI responses with built-in text-to-speech, perfect for hands-free use while driving or multitasking.
- **Model Hub** — Browse, download, and manage GGUF models from a curated list with one-tap setup and progress tracking.
- **GPU Acceleration** — Automatically leverages Snapdragon and Mali GPU offload via llama.cpp for faster token generation.
- **System Monitor** — Real-time stats showing tokens per second, generation time, and token count so you can benchmark performance.

## Why LlamaBox?

- **Privacy by design** — Unlike cloud AI services, every inference happens locally; your chat history never leaves your device.
- **No accounts, no friction** — Skip sign-ups, subscriptions, and API keys. Just install, download a model, and start chatting.
- **Works anywhere** — Airplanes, remote areas, or low-connectivity environments — your on-device LLM is always available.

## How it works

LlamaBox bundles [llama.cpp](https://github.com/ggerganov/llama.cpp) and [llama.rn](https://github.com/myllama/llama.rn) to run quantized GGUF models directly on your Android phone's CPU and GPU. The app downloads model files to local storage, loads them into memory, and performs inference entirely on-device through a React Native interface optimized for mobile hardware.

## Get access

LlamaBox is currently in **closed beta** on Google Play. The source code is not yet public, but you can request early access by sending an email to **[aalhad.dev@gmail.com](mailto:aalhad.dev@gmail.com)** with the subject **"LlamaBox beta access"**. There are no install commands or build instructions available at this time.

## Tech stack

- **React Native** `0.81` — Cross-platform UI framework with New Architecture enabled
- **Expo SDK** `~54.0.0` — Development workflow and native API access
- **llama.rn** `0.12.0-rc.8` — React Native bindings for llama.cpp on-device inference
- **llama.cpp** (via llama.rn) — High-performance quantized GGUF model execution on CPU/GPU
- **expo-sqlite** `~15.0.0` — Local chat history and message persistence
- **expo-file-system** `~19.0.0` — Secure model file storage and cache management
- **expo-image-picker** `~16.0.0` — Image selection for multimodal vision chat
- **Zustand** — Lightweight state management for the React Native LLM UI

## Roadmap

*Items below are tentative and subject to change.*

- Expanded model presets and one-click import for custom GGUF files
- iOS port exploration and Apple Silicon GPU acceleration research
- Plugin / tool-use system for calculator, web-search, and code execution
- DeepSeek, Qwen, and Gemma vision model preset packs
- Performance tuning guides and automatic context-window sizing
- Open-source release and community-driven feature voting

## Contributing

Contributions will be welcomed once the source code is made public. Because LlamaBox is dual-licensed, all contributors must sign a Contributor License Agreement (CLA) so that we can continue offering both the free AGPL-3.0 release and a separate commercial license. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for the full policy before opening a pull request.

## License & trademark

LlamaBox is **dual-licensed**:

- **[AGPL-3.0](LICENSE)** — Free, copyleft open-source use.
- **Commercial license** — Available for closed-source commercial derivatives. Contact [aalhad.dev@gmail.com](mailto:aalhad.dev@gmail.com) for pricing and terms.

> **Trademark notice:** "LlamaBox" is a reserved trademark of the LlamaBox project. The name may not be used to endorse or promote derived works without written permission.

## Links

- **Live site:** https://llamabox-ai.github.io/
- **GitHub org:** https://github.com/llamabox-ai
- **Privacy policy:** https://llamabox-ai.github.io/privacy.html
- **Contact:** [aalhad.dev@gmail.com](mailto:aalhad.dev@gmail.com)
