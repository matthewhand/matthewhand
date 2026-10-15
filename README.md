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
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | F5-TTS-backed OpenAI-style speech API with voice selection, experimental sentence-level PCM streaming, and estimated timestamps. | **Experimental alpha.** Streaming is implemented on public `main`, but its concurrency safeguards and current model-backed/Docker operation remain unverified end to end; timestamps are not forced alignment. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | OpenAI-style speech endpoint built around Kokoro TTS. | **Experimental.** Published output, authorization and integration behavior require verification. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for Llama Stack model lists and non-streaming chat completions. | **Legacy prototype.** Current compatibility, streaming and deployment unverified. |

A synthetic preview is not a live camera or inference test, and an unmerged draft is not a release. These labels describe public evidence, not production certification.

## Private desktop prototypes

Omarchy applets and Cadence. Private, not installable from a public URL. Not hexagon-kit demos. Captures are from this machine on 15 October 2026. There is no automated test suite for these READMEs.

Still open, and the only Omarchy work that matters until it is done:

- After sleep, the USB hub that holds the Surface keyboard and the Nano dongle can drop and stay gone. The power rule does not bring it back. A resume hook exists and is not installed yet, because installing it needs root.
- Cadence's rotation gif is five frames of a wordmark, not a slide rotation. The name, a clean install, and that claim are still open issues.
- Dictation was only captured idle. Deskflow was not connected, and the portal grant was not exercised. The OSK-toggle gif includes a permission dialog.
- The AI-config bar button is unused. The archived `omarchy-osk` fork stays archived. The compositor touch plugin stays unloaded.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
