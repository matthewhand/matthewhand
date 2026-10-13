# Hey, I'm matthewh

I work on a personal [Omarchy](https://omarchy.dev) desktop and the tooling around
it — an AI-assisted setup where the agent tooling, the window manager config and
the desktop itself are all first-class citizens.

Most of what I publish is small and specific. The maturity column is meant
honestly: I'd rather label something **alpha** than imply it's finished.

## Built from scratch

| Project | What it does | Maturity |
|---|---|---|
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Original Flask integration exposing Kokoro TTS through OpenAI-style speech and model-list endpoints, built around a third-party Kokoro model. Includes ONNX and Docker experiments; optional GPU providers are proposed in PR #2. | **Experimental / repair required.** Source-only audit found speech output-contract, Docker build, API authorization and README discrepancies. Prior live CPU speech evidence exists, but published `main` is not independently verified as runnable. Not production-ready. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local-first camera snapshot archive. A Python watched-folder preview indexes JPEGs, groups frames into visits and serves a browser timeline; a separate refined dashboard uses fictional fixtures. Object detection and vision-model decisions remain future integrations. | **Alpha — synthetic MVP preview.** Published demonstration: 10 fictional JPEGs grouped into 7 visits. No production camera integration or actual model inference demonstrated. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Small Nginx/njs adapter intended to translate Llama Stack model-list and non-streaming chat-completion responses into OpenAI-style JSON. Docker Compose example included; streaming is still a TODO. | **Experimental / legacy prototype.** Source-only review: no published automated tests or verified working deployment; configuration, build, compatibility and security gates remain open. Not production-ready. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Python MCP server that connects clients to Flowise chatflows. Offers FastMCP tools to list chatflows and request predictions, plus low-level dynamic per-chatflow tools. | **Experimental / pre-release.** Source-only review finds tool-authorization, stdio logging, configuration and HTTP error-handling gaps. Not production-ready; assistant integration unverified here. |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** ⭐ 156 | MCP server that dynamically exposes REST APIs described by OpenAPI specs. Dual-stack MCP 1.x / 2.x, with native Streamable HTTP so stateless POST `/mcp` works behind round-robin load balancing without sticky sessions. | **Stable** — v0.4.0, 2026-09-05. The one here I'd actually point you at. |
| **[omarchy-screensaver-cadence](https://github.com/matthewhand/omarchy-screensaver-cadence)** | Fork of Omarchy's screensaver into a rotating ASCII display. A slide list instead of one static file: `text`, `image`, `images DIR`, `exec` and `notify` slides, each with its own dwell time, and slides can pick their own `ttfx` effect and gradient per rotation. | **Alpha** — works on one machine only. See the honest limits below. |

### Why "alpha" and not "beta"

`omarchy-screensaver-cadence` is alpha because beta would overstate it. It has an
installer, a README and a fresh-install smoke test, but:

- **One user, one machine.** No external testers.
- **Two paths are unverified.** The Omarchy menu override parses without error but
  I've never seen it render in the menu, and the herdr slide has never run with
  herdr actually up — so its status-driven colouring is untested.
- **Bugs found and fixed during bring-up**, including a `parse_conf` that appended
  instead of resetting (duplicating every slide on each rescan) and an `install.sh`
  that still referenced pre-rename scripts after a rename.

It builds *on* `omarchy-branding-screensaver` and `omarchy-transcode-ascii` rather
than replacing them, and touches nothing in `/usr/share/omarchy`.

## Forked

| Project | Upstream | What I did | Maturity |
|---|---|---|---|
| `holman-linux-python` | `scottmckenzie/holman-linux-python` — **no longer public** | Public fork preserved for reference; not contributed upstream. The upstream repo has since disappeared, so no patch can be diffed or credited. | **Public fork; experimental.** Treat this as an unfinished copy, not an upstream-maintained release. |

I also carry private mirrors of several upstream projects I use on the desktop
(an `xdg-desktop-portal-hyprland` fork with `RemoteDesktop` support, plus a
Deskflow source mirror), kept private so I can patch them without upstream noise.

## Notes

- Some desktop tools remain private. The directory below lists the remaining public repositories; OpenAI Kokoro TTS, Funes Vision, Llama Stack Bridge and MCP Flowise are featured above.
- Anything labelled stable above is something I'd use again tomorrow. Anything
  labelled alpha is a work in progress that happens to be public.

## Public repository directory
_Public repository navigation updated on 13 October 2026. OpenAI Kokoro TTS, Funes Vision, Llama Stack Bridge and MCP Flowise are featured above; the remaining public repositories are listed below. Private repositories are excluded. A listing is not a statement that a project is release-ready._

### Other original projects (10)
| Repository | Description |
|---|---|
| [matthewhand](https://github.com/matthewhand/matthewhand) | Profile README for matthewhand |
| [matthewhand.github.io](https://github.com/matthewhand/matthewhand.github.io) | Public repository |
| [mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy) | MCP server that dynamically exposes REST APIs defined by OpenAPI specs. Dual-stack MCP 1.x/2.x with native Streamable HTTP. |
| [omarchy-deskflow-applet](https://github.com/matthewhand/omarchy-deskflow-applet) | Public repository |
| [omarchy-screensaver-cadence](https://github.com/matthewhand/omarchy-screensaver-cadence) | Rotating ASCII display for Omarchy: text, image, live data and notification slides |
| [open-webui-integrations](https://github.com/matthewhand/open-webui-integrations) | Public repository |
| [openai-f5-tts](https://github.com/matthewhand/openai-f5-tts) | This project provides a Flask-based API for generating high-quality text-to-speech (TTS) audio using F5-TTS, a flexible and powerful TTS engine. The API supports cus |
| [operating-swarm](https://github.com/matthewhand/operating-swarm) | Operating Swarm (OS): provider-agnostic agent operating layer and harness. Native execution, external harnesses, and peer OS instances as one abstraction. |
| [perplexica-aws](https://github.com/matthewhand/perplexica-aws) | Public repository |
| [snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit) | Shared Hexagon NPU runtime kit for first-generation Copilot+ PCs: hardware probe, model catalog, XDG cache, and preflight. |

### Forks and upstream experiments (38)
| Repository | Description |
|---|---|
| [accept-a-payment](https://github.com/matthewhand/accept-a-payment) | Learn how to accept a payment from customers around the world with a variety of payment methods. |
| [amd-strix-halo-image-video-distrobox](https://github.com/matthewhand/amd-strix-halo-image-video-distrobox) | ROCm distrobox/Docker environment for image & video generation (Qwen Image/Edit, WAN 2.2, LTX-2, ComfyUI) on AMD Strix Halo / gfx1151 · **Archived** |
| [ansible_role_microk8s](https://github.com/matthewhand/ansible_role_microk8s) | Ansible role to install microk8s on ubuntu |
| [audio.cpp-hub](https://github.com/matthewhand/audio.cpp-hub) | Web GUI for audio.cpp |
| [chatterbox](https://github.com/matthewhand/chatterbox) | Public fork |
| [ChatterCraft-Pinokio](https://github.com/matthewhand/ChatterCraft-Pinokio) | ChatterCraft is a Gradio app that integrates an LLM for story generation with ChatterBox TTS voice cloning. Users can create unique stories from prompts or input tex |
| [Chattered](https://github.com/matthewhand/Chattered) | All in one Gradio interface for chatterbox. Voice cloning from uploaded audio samples, automatic text processing for long content and real-time speech generation wit |
| [docker-compose-ui](https://github.com/matthewhand/docker-compose-ui) | web interface for Docker Compose |
| [GroqCasters](https://github.com/matthewhand/GroqCasters) | Public fork |
| [herdr](https://github.com/matthewhand/herdr) | the runtime your coding agents live on |
| [holman-linux-python](https://github.com/matthewhand/holman-linux-python) | Holman SDK for Python on Linux |
| [htpc-download-box](https://github.com/matthewhand/htpc-download-box) | Sonarr / Radarr / Jackett / NZBGet / Deluge / OpenVPN / Plex |
| [InkMemories](https://github.com/matthewhand/InkMemories) | A cloud-powered, eInk, smart photo frame. |
| [labs-Voice-Agent](https://github.com/matthewhand/labs-Voice-Agent) | A fully opensource framework for building and evaluating voice agents with open models. |
| [MagicQuill](https://github.com/matthewhand/MagicQuill) | An intelligent, interactive Image Editing System. Easily erase and add objects on a user-friendly interface. |
| [omarchy-chronos](https://github.com/matthewhand/omarchy-chronos) | Omarchy bar clock whose calendar has a pulse — day-progress ring, drawn moon phase, shimmering year/life rails, staggered month grid. A fork of omarchy.clock. |
| [omarchy-osk](https://github.com/matthewhand/omarchy-osk) | Public fork |
| [omniplex](https://github.com/matthewhand/omniplex) | Open-Source Perplexity |
| [open-webui](https://github.com/matthewhand/open-webui) | User-friendly AI Interface (Supports Ollama, OpenAI API, ...) |
| [openaudio](https://github.com/matthewhand/openaudio) | Public fork |
| [OpenMausBot](https://github.com/matthewhand/OpenMausBot) | Public fork |
| [openmuse-1](https://github.com/matthewhand/openmuse-1) | A personal agent with a browser, terminal, files, and work that keeps going built with CopilotKit and AG-UI. |
| [openwebui-docs](https://github.com/matthewhand/openwebui-docs) | https://docs.openwebui.com |
| [Orpheus-TTS-FastAPI](https://github.com/matthewhand/Orpheus-TTS-FastAPI) | Public fork |
| [persona](https://github.com/matthewhand/persona) | Bringing real-time voice to life. |
| [rakazo](https://github.com/matthewhand/rakazo) | Open-source Grok Bot alternative. Choose your own model and sandbox. |
| [rift](https://github.com/matthewhand/rift) | 󰦛 Rift: native Omarchy bar plugin that remembers which apps belong on a workspace and brings them back in one click. No geometry. Hyprland tiles, Rift remembers. |
| [self-hosted-ai-starter-kit](https://github.com/matthewhand/self-hosted-ai-starter-kit) | The Self-hosted AI Starter Kit is an open-source template that quickly sets up a local AI environment. Curated by n8n, it provides essential tools for creating secur |
| [server-wp-mcp](https://github.com/matthewhand/server-wp-mcp) | Public fork |
| [stripe-checkout-next-js-demo](https://github.com/matthewhand/stripe-checkout-next-js-demo) | Public fork |
| [talkbot](https://github.com/matthewhand/talkbot) | Text-to-speech and translation bot for Discord |
| [trueforge](https://github.com/matthewhand/trueforge) | The open-source agent harness - the runtime layer that turns an LLM into a working agent. |
| [ugv_rpi](https://github.com/matthewhand/ugv_rpi) | Raspberry Pi example for the WaveShare UGV robots: WAVE ROVER, UGV Rover, UGV Beast, RaspRover, UGV01, UGV02. |
| [Ultimate-TTS-Studio](https://github.com/matthewhand/Ultimate-TTS-Studio) | 🟢 NVIDIA ONLY – All-in-One TTS App with Kokoro, KittenTTS, Higgs audio, Chatterbox, Fish-Speech, F5 & index-tts & indextts2, Supports Conversation Mode & eBook-to-Au |
| [vectara-ingest](https://github.com/matthewhand/vectara-ingest) | An open source framework to crawl data sources and ingest into Vectara |
| [vibevoice-realtime](https://github.com/matthewhand/vibevoice-realtime) | Public fork |
| [VoiceMem](https://github.com/matthewhand/VoiceMem) | Infrastructure for the next generation of voice agents, designed to provide universal memory. It is divided into a left brain and a right brain, storing information  |
| [webxr-samples](https://github.com/matthewhand/webxr-samples) | Samples to demonstrate use of the WebXR Device API |

