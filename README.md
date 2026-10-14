# Hey, I'm matthewh

I build local-first AI tools, agent workflows, speech integrations and desktop experiments. On my [Omarchy](https://omarchy.org/) desktop, the window manager and the tooling around it are part of the project.

## Selected projects

A curated mix of original projects and substantial work on upstream foundations, with attribution in the linked repositories. Status labels refer to **public main**, not private branches or unmerged drafts.

| Project | Purpose | Maturity |
|---|---|---|
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | Turns OpenAPI-described REST endpoints into MCP tools over Streamable HTTP or stdio. | **Established, versioned.** v0.4.0 source tag and PyPI package; latest published GitHub Release: **v0.3.3**. |
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer evolved from OpenAI's experimental Swarm, with API, CLI, WebUI and external harness integrations. | **Experimental alpha.** Main has advanced beyond its published package; architecture remains in transition. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-folder browser for JPEG snapshots and grouped visits. | **Alpha synthetic MVP.** 10 fictional frames grouped into 7 visits; live camera and model inference not demonstrated. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python toolkit for Snapdragon hardware/provider discovery, model caching and resource preflight. | **Alpha, v0.3.0 candidate.** Live Hexagon/QNN inference and a public PyPI release remain unverified. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Exposes Flowise chatflows through Model Context Protocol tools. | **Experimental.** Published integration and authorization behavior need verification. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | OpenAI-style speech API built around F5-TTS, with voice options and estimated timestamps. | **Experimental alpha.** Public-main runtime and deployment behavior not independently reverified; timestamps are not forced alignment. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | OpenAI-style speech endpoint built around Kokoro TTS. | **Experimental.** Published output, authorization and integration behavior require verification. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for Llama Stack model lists and non-streaming chat completions. | **Legacy prototype.** Current compatibility, streaming and deployment unverified. |

A synthetic preview is not a live camera or inference test, and an unmerged draft is not a release. These labels describe public evidence, not production certification.

## Private desktop prototypes

Omarchy bar applets and the Cadence screensaver. Private repos, not installable from a public URL. Evidence is from this machine on 15 October 2026. None of these are hexagon-kit demos.

| Project | What it is | What was actually captured |
|---|---|---|
| Snippet pad | Left-edge pad: saved entries, a keypad, and a voice row that can hand text to the agent. | The open pad, including the keypad, voice row, and on-screen-keyboard row. Dictation was not started and the AI buttons were not pressed. |
| Deskflow applet | Deskflow client controls: host, connect, auto-connect, and a remote-control grant file for a patched portal. | The open panel. The server address is covered. Allow remote control and auto-connect were off. Nothing was connected or toggled. |
| System load | CPU percentage from `/proc/stat`, click focuses `btop`. | The bar glyph, plus four frames where the percentage changes. `btop` was not opened. |
| Dictation | Voxtype start/stop on a bar mic. | The idle glyph only. Recording was not started. |
| OSK toggle | Bar button for the on-screen keyboard. | An older gif in the private repo shows the keyboard. That frame also includes a permission dialog, so it is not a clean demo. |
| Cadence | Rotating ASCII screensaver: text, image, exec, and notification slides, plus cached AI text. | `hero.gif` (2 October) is a braille smiley and a clock. `hero-rotation.gif` is five frames of a dotted SurfaceBook wordmark, not a full slide rotation. Private issues for the name, a clean install, and the README claims are still open. |

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
