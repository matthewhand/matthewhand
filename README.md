# Hey, I'm matthewh

I build local-first AI tools, agent workflows and useful apps, spanning speech, vision, automation and hardware integration.

My projects and integrations are listed first, followed by selected upstream contributions.

**Quick links:** [AI Infrastructure](#ai-infrastructure) · [Hardware & Input](#hardware--input) · [Android TV Apps](#android-tv-apps) · [Self-hosted Web Apps](#self-hosted-web-apps) · [Open-source contributions](#open-source-contributions)

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/section-divider.svg" alt="" width="600">

## AI Infrastructure

<img src="https://raw.githubusercontent.com/matthewhand/mcp-openapi-proxy/main/docs/assets/mcp-openapi-proxy-banner.png" alt="OpenAPI endpoints become LLM tools through MCP OpenAPI Proxy" width="600">

Repo: [matthewhand/mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)

OpenAPI-described REST APIs as MCP tools over Streamable HTTP or stdio.

---

<img src="https://raw.githubusercontent.com/matthewhand/mcp-flowise/efc65803bf2613943e6e46cbc75cf829cceff573/docs/assets/mcp-flowise-banner.png" alt="MCP clients discover and run Flowise chatflows through mcp-flowise" width="600">

Repo: [matthewhand/mcp-flowise](https://github.com/matthewhand/mcp-flowise)

Discover and run Flowise chatflows from MCP clients, with authentication and flow filtering.

---

<img src="https://raw.githubusercontent.com/matthewhand/openai-f5-tts/f9f2a70a577eb4d27d36577f4e9eb7fea592e08f/docs/assets/openai-f5-tts-banner.png" alt="An OpenAI-compatible TTS API runs the F5-TTS model to generate speech" width="600">

Repo: [matthewhand/openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)

Independent F5-TTS API wrapper for self-hosted speech, selectable voices, custom checkpoints, sentence-level PCM streaming and estimated timestamps.

---

<img src="https://raw.githubusercontent.com/matthewhand/openai-kokoro-tts/103494493a7660286ab23ae009cef37a8ce44cfe/docs/assets/openai-kokoro-tts-banner.png" alt="An OpenAI-compatible TTS API runs the Kokoro model to generate speech" width="600">

Repo: [matthewhand/openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)

Independent, CPU-first OpenAI-compatible speech API around Kokoro and kokoro-onnx.

---

<img src="https://raw.githubusercontent.com/matthewhand/llama-stack-bridge/594b8209dbd498f06a9eac2d483e3f570b10f6a7/docs/assets/llama-stack-bridge-banner.png" alt="OpenAI-style clients connect to Llama Stack through llama-stack-bridge" width="600">

Repo: [matthewhand/llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)

Nginx/njs adapter for Llama Stack model lists and non-streaming chat.

<br>

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/section-divider.svg" alt="" width="600">

## Hardware & Input

<img src="https://raw.githubusercontent.com/matthewhand/open-wiimote/main/docs/images/open-wiimote.svg" alt="OpenWiimote: bring your Wii Remote back into play" width="600">

Repo: [matthewhand/open-wiimote](https://github.com/matthewhand/open-wiimote)

Wii Remote buttons and tilt as a virtual gamepad on Linux, with desktop and browser interfaces.

---

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/waltop-osx-banner.png" alt="waltop-osx: pen pressure for macOS" width="600">

Repo: [matthewhand/waltop-osx](https://github.com/matthewhand/waltop-osx)

Userspace pen-pressure support for the WALTOP Slim Tablet 12.1 on macOS.

<br>

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/section-divider.svg" alt="" width="600">

## Android TV Apps

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/kinegra-home-banner-wide.png" alt="Kinegra Home: two apps on one Android TV screen" width="600">

Repo: [matthewhand/kinegra-home](https://github.com/matthewhand/kinegra-home)

Adjustable side-by-side Split View and remote session controls for NVIDIA SHIELD.

---

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/kinegra-amp-banner-wide.png" alt="Kinegra Amp: music and visuals for NVIDIA SHIELD" width="600">

Repo: [matthewhand/kinegra-amp](https://github.com/matthewhand/kinegra-amp)

Music Assistant and local-file player with queues, audio-reactive visuals and optional webcam avatars.

<br>

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/section-divider.svg" alt="" width="600">

## Self-hosted Web Apps

### [funes&#8209;vision](https://github.com/matthewhand/funes-vision)

Local watched-folder browser for JPEG snapshots and grouped visits, with a demo gallery.

---

### [operating&#8209;swarm](https://github.com/matthewhand/operating-swarm)

Agent workflows across model APIs, agent CLIs and remote harnesses, with an API, CLI and WebUI.

---

### [Trackie Assistant](https://github.com/matthewhand/trackie-assistant)

Archive permitted public Suno tracks locally, with a WebUI, CLI and Home Assistant add-on.

<br>

<img src="https://raw.githubusercontent.com/matthewhand/matthewhand/main/assets/section-divider.svg" alt="" width="600">

## Open-source contributions

### Merged upstream

| Project | Contribution |
|---|---|
| <h3><a href="https://github.com/open-webui/open-webui">Open&nbsp;WebUI</a></h3> | Added Qdrant Cloud API-key authentication. **Merged:** [#6954](https://github.com/open-webui/open-webui/pull/6954). |
| <h3><a href="https://github.com/open-webui/docs">Open&nbsp;WebUI&nbsp;Docs</a></h3> | HTTPS/Nginx setup, a RAG tutorial and a restructured Getting Started guide. **Merged:** [#257](https://github.com/open-webui/docs/pull/257), [#260](https://github.com/open-webui/docs/pull/260), [#266](https://github.com/open-webui/docs/pull/266). |

### Under review

| Project | Contribution |
|---|---|
| <h3><a href="https://github.com/scottmckenzie/holman-linux-python">Holman&nbsp;Linux&nbsp;SDK</a></h3> | BX2 MK1 discovery and dual-outlet control. **Open:** [#9](https://github.com/scottmckenzie/holman-linux-python/pull/9). |
| <h3><a href="https://github.com/CopilotKit/openmuse">OpenMuse</a></h3> | Contributed the local-persistence implementation in [#94](https://github.com/CopilotKit/openmuse/pull/94), now carried forward by another contributor in **open** continuation [#166](https://github.com/CopilotKit/openmuse/pull/166). |
| <h3><a href="https://github.com/emzimmer/server-wp-mcp">WordPress&nbsp;MCP</a></h3> | Added the package executable entry so the server can run directly from GitHub through npx. **Open:** [#5](https://github.com/emzimmer/server-wp-mcp/pull/5). |

See each repository and its upstream documentation for current setup, platform support and limitations. Models, dependencies and assets retain their own licence terms.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
