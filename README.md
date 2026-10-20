# Hey, I'm matthewh

I build local-first AI tools, agent workflows, speech integrations and desktop experiments. On my [Omarchy](https://omarchy.org/) desktop, the window manager and the tooling around it are part of the project.

## Selected projects

A curated mix of original projects and substantial work on upstream foundations, with attribution in the linked repositories. Status labels refer to **public main**, not private branches or unmerged drafts.

| Project | Purpose | Maturity |
|---|---|---|
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | Turns OpenAPI-described REST endpoints into MCP tools over Streamable HTTP or stdio. | **Established, versioned.** v0.4.0 tagged source, PyPI package and [published GitHub Release](https://github.com/matthewhand/mcp-openapi-proxy/releases/tag/v0.4.0). |
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer evolved from OpenAI's experimental Swarm, with API, CLI, WebUI and external harness integrations. | **Experimental alpha.** Main has advanced beyond its published package; architecture remains in transition. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-folder browser for JPEG snapshots and grouped visits. | **Alpha synthetic MVP.** 10 fictional frames grouped into 7 visits; live camera and model inference not demonstrated. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python toolkit for Snapdragon hardware/provider discovery, model caching and resource preflight. | **Alpha, v0.3.0 candidate.** Live Hexagon/QNN inference and a public PyPI release remain unverified. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Exposes Flowise chatflows through Model Context Protocol tools. | **Experimental.** Published integration and authorization behavior need verification. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | **Self-hosted speech for AI assistants and voice apps.** Independently developed OpenAI-style API wrapper around upstream F5-TTS, with selectable voices, support for your own trained or fine-tuned checkpoints, sentence-level PCM streaming, and estimated timestamps. | **SOHO-oriented community beta, verified on one machine.** NVIDIA GPU speech generation verified in Docker Desktop on 20 October 2026: Scarlett (v0) and Emilia (v1), non-streaming WAV/MP3, incremental sentence streaming, estimated timestamps, and authentication. Generated speech was transcribed correctly. Intended for trusted, sequential use; simultaneous streaming and cancellation during inference remain unverified. Upstream pretrained weights are noncommercial; custom-checkpoint rights depend on their provenance. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Independently developed OpenAI-compatible API wrapper around the upstream Kokoro TTS model; not affiliated with OpenAI or the Kokoro authors. | **Community beta, verified on one machine.** CPU and NVIDIA CUDA speech generation verified in Docker Desktop on 20 October 2026, including WAV/MP3 output and bearer authentication. CPU image contains no CUDA packages. AMD and other accelerators remain unverified; see the [verification report](https://github.com/matthewhand/openai-kokoro-tts/blob/main/docs/verification-2026-10-20.md). |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for Llama Stack model lists and non-streaming chat completions. | **Legacy prototype.** Current compatibility, streaming and deployment unverified. |
| **[waltop-osx](https://github.com/matthewhand/waltop-osx)** | Userspace macOS shim that restores pen pressure for the WALTOP Slim Tablet 12.1" (USB 172f:0031), whose firmware mislabels its pressure field. | **Working on one machine.** Verified drawing with pressure in Krita on one Intel Mac (macOS 14.8.7) with one tablet; Apple Silicon, other macOS versions and other apps untested. |

A synthetic preview is not a live camera or inference test, and an unmerged draft is not a release. These labels describe public evidence, not production certification.

## Private desktop prototypes

Omarchy applets and Cadence. Private, not installable from a public URL. Not hexagon-kit demos. Captures are from this machine on 15 October 2026. There is no automated test suite for these READMEs.

Still open, and the only Omarchy work that matters until it is done:

- After sleep, the USB hub that holds the Surface keyboard and the Nano dongle can drop and stay gone. The power rule does not bring it back. A resume hook exists and is not installed, because installing it needs a typed root password. Touch after suspend is a separate failure. The compositor touch plugin stays unloaded.
- Cadence's rotation gif is five frames of a wordmark, not a slide rotation. The GitHub repository has not been renamed. A temporary-home install was tested and leaves `shell.json` alone. Idle stays on Omarchy's screensaver until the opt-in shim is installed. The screensaver was not launched.
- Dictation was only captured idle. Deskflow was not connected, and the portal grant was not exercised. The OSK-toggle gif includes a permission dialog.
- The AI-config bar button stays disabled. Its opener is covered by fixture tests. The archived `omarchy-osk` fork stays archived.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
