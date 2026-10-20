# LMPanel

**[中文](./README.md) | English**

**A local LLM management panel that gives your AI coding agents free, private local models.**

Model download, deep parameter tuning, one-click model switching, and a built-in terminal — all in one panel. No paid APIs, and your data never leaves your machine.

---

## Why LMPanel

AI coding agents (Claude, Gemini, OpenAI, etc.) calling cloud models cost money, raise privacy concerns, and depend on network access. LMPanel lets you run local models on **your own computer** and connect them to your agents through a standard interface:

- **Free**: local inference, zero cost
- **Private**: models and data stay on your machine
- **Flexible**: switch between multiple models anytime — pick the best one for each task

## Quick Start

1. **Download**: use any option below to get the installer
2. **Install**: double-click and click through (custom install path supported)
3. **Use**: download a model → configure parameters → start it → **one-click sync to Agent**, or manually enter the local address

## Download

- **Option 1 (recommended)**: get the latest installer from **GitHub Releases** (Windows 10/11, 64-bit) — click **Releases** on the right side of the page and download `LMPanel_1.0.0_x64-setup.exe` (a `LMPanel_1.0.0_x64_en-US.msi` is also available for enterprise deployment)
- **Option 2 (faster in China)**: Quark Cloud Drive: <https://pan.quark.cn/s/6b6aaf9dfbbb>

> **System requirements**: Windows 10 / 11 (64-bit). A local inference engine is installed on first use with one click from within the panel.
> If automatic download is slow, grab the **backend pack** (Quark Cloud Drive, same folder as the installer) and extract it into the software's backend directory (see Settings for its location).

## Supported Backends

LMPanel manages the following inference engines (view/upgrade in Settings):

- **llama.cpp** — local LLM inference engine (chat / AI coding agent)
- **stable-diffusion.cpp** — local image generation (Stable Diffusion)
- **llama-swap** — multi-model switching gateway (route multiple models by name)
- **audio.cpp** — local audio model inference (audio chat / understanding)
- **whisper.cpp** — local speech recognition (Whisper, speech-to-text)

## Features

- **Model download**: built-in search & download with resume support and integrity verification
- **Deep parameter tuning**: visual control of sampling, performance, memory, etc., with one-click presets
- **One-click model switching**: route multiple models by name — switch seamlessly
- **Built-in terminal**: one-click model start, live logs, smart startup-failure diagnostics
- **Ready to go**: single instance, system tray, global shortcut (Ctrl+Shift+L)
- **Auto-update**: checks for new versions in the background, one-click install
- **Bilingual UI (EN/CN)**, dark & light themes

## Auto-Update

LMPanel automatically checks for new versions: it downloads in the background and prompts you to install in one click — no need to reinstall manually, and your data and configuration are preserved.

## FAQ

- **Why do I need to install a component on first use?** Running models requires a local inference engine; the panel guides you through a one-click install on first launch.
- **Model downloads are slow?** Switch the download source (Hugging Face / ModelScope) — ModelScope is recommended on China mainland networks.
- **How do I let my AI agents use local models?** After starting a model, click **one-click sync to Agent** in Settings to write them into configured agents, or manually enter the local address (`http://127.0.0.1:<port>/v1`) as the agent's baseURL.

## License

MIT — see LICENSE.

## Acknowledgements

Thanks to the following open-source projects that make LMPanel possible:

- [llama.cpp](https://github.com/ggml-org/llama.cpp) — local LLM inference engine
- [llama-swap](https://github.com/mostlygeek/llama-swap) — multi-model hot-swap gateway
