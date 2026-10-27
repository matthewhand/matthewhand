# Hey, I'm matthewh

I build local-first AI tools, agent workflows, speech integrations and desktop experiments. On my [Omarchy](https://omarchy.org/) desktop, the window manager and the tooling around it are part of the project.

## Selected projects

A curated mix of original projects and substantial work on upstream foundations, with attribution in the linked repositories. Status labels refer to **public main**, not private branches or unmerged drafts.

| Project | Purpose | Maturity |
|---|---|---|
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | Turns OpenAPI-described REST endpoints into MCP tools over Streamable HTTP or stdio. | **Established, versioned.** v0.4.0 tagged source, PyPI package and [published GitHub Release](https://github.com/matthewhand/mcp-openapi-proxy/releases/tag/v0.4.0). |
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Coordinates model APIs, local agent CLIs and remote harnesses through a shared API, CLI and WebUI. Evolved from OpenAI's experimental Swarm. | **Experimental alpha.** A model-and-tool workflow is verified; integration coverage varies, and the published package lags source. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-folder browser for JPEG snapshots and grouped visits. | **Public alpha (synthetic-only).** Public `main` demonstrates 10 fictional JPEGs grouped into 7 visits, without live cameras or model inference. **Separate private deployment (verified 23 October 2026):** active camera-ingestion pipelines and gallery/API with YOLOv4-tiny (OpenCV) object detection; optional deep vision/LLM decisions currently disabled. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Lets MCP clients discover and run Flowise chatflows, with authentication and flow filtering. | **Experimental.** Core chatflow integration verified. [Verification details](https://github.com/matthewhand/mcp-flowise/blob/main/docs/verification-2026-10-20.md). |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | **Self-hosted speech for AI assistants and voice apps.** Independently developed OpenAI-style API wrapper around upstream F5-TTS, with selectable voices, support for your own trained or fine-tuned checkpoints, sentence-level PCM streaming, and estimated timestamps. | **SOHO-oriented community beta, verified on one machine.** NVIDIA GPU speech generation verified in Docker Desktop on 20 October 2026: the author's privately trained Scarlett (v0, not distributed) and upstream Emilia (v1), non-streaming WAV/MP3, incremental sentence streaming, estimated timestamps, and authentication. Generated speech was transcribed correctly. Intended for trusted, sequential use; simultaneous streaming and cancellation during inference remain unverified. Upstream pretrained weights are noncommercial; custom-checkpoint rights depend on their provenance. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Independently developed OpenAI-compatible API wrapper around the upstream Kokoro TTS model; not affiliated with OpenAI or the Kokoro authors. | **Community beta, verified on one machine.** CPU and NVIDIA CUDA speech generation verified in Docker Desktop on 20 October 2026, including WAV/MP3 output and bearer authentication. CPU image contains no CUDA packages. AMD and other accelerators remain unverified; see the [verification report](https://github.com/matthewhand/openai-kokoro-tts/blob/main/docs/verification-2026-10-20.md). |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for Llama Stack model lists and non-streaming chat completions. | **Legacy prototype.** Current compatibility, streaming and deployment unverified. |
| **[waltop-osx](https://github.com/matthewhand/waltop-osx)** | Userspace macOS shim that restores pen pressure for the WALTOP Slim Tablet 12.1" (USB 172f:0031), whose firmware mislabels its pressure field. | **Working on one machine.** Verified drawing with pressure in Krita on one Intel Mac (macOS 14.8.7) with one tablet; Apple Silicon, other macOS versions and other apps untested. |

A synthetic preview is not a live camera or inference test, and an unmerged draft is not a release. These labels describe public evidence, not production certification.

## Projects in development

These are broad areas of ongoing work, not claims that every prototype is released or production-ready. Individual projects vary in maturity; public repositories above provide examples where available.

| Area | Focus |
|---|---|
| **Cross-Platform Desktop Experiences** | Omarchy-inspired desktop workflows across Linux, macOS, Asahi Linux and Windows, including touch, pen and accessible interaction. |
| **Edge AI & Hardware Acceleration** | Local multimodal AI on consumer hardware, including Snapdragon NPUs, NVIDIA Tegra and AMD GPUs; accelerator claims require measured evidence. |
| **Embodied AI & Interactive Systems** | Robotics, speech, computer vision, Kinect and alternative controllers for physical and expressive interaction. |
| **Smart Home & Intelligent Automation** | Home Assistant, presence sensing, local media workflows and AI-assisted home operations. |
| **Parametric Design & Digital Fabrication** | Functional OpenSCAD design, practical 3D printing, mechanical parts and AI-assisted CAD workflows. |
| **AI Infrastructure & Developer Tools** | Agent orchestration, MCP interoperability, API gateways, local model services and developer tooling. |

Development work may be private or experimental. A theme here is not a statement of public availability or hardware certification.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
