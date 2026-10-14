# Hey, I'm matthewh

I work on a personal [Omarchy](https://omarchy.dev) desktop and the tooling around
it — an AI-assisted setup where the agent tooling, the window manager config and
the desktop itself are all first-class citizens.

Most of what I publish is small and specific. The maturity column is meant
honestly: I'd rather label something **alpha** than imply it's finished.

## Projects I've built or substantially developed

A curated selection of original projects and significant derivative work, with upstream origins acknowledged where applicable.

| Project | What it does | Maturity |
|---|---|---|
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer evolved from OpenAI's experimental Swarm, with a Django API, CLI/WebUI, blueprints, handoffs and external-harness adapters. | **Experimental alpha (`main`).** Published v0.5.4 predates newer source work; the API/Blueprint separation remains incomplete, and the latest public `main` run includes a failed Python Tests workflow. Not independently production-validated. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python library for Snapdragon Copilot+ hardware detection, model caching, resource preflight, CLI and application status reporting. | **Alpha / pre-release (0.3.0 candidate).** Source and synthetic tests available; live QNN execution and public package release not independently verified. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Original Flask integration exposing Kokoro TTS through OpenAI-style speech and model-list endpoints, built around a third-party Kokoro model. Includes ONNX and Docker experiments; optional GPU providers are proposed in PR #2. | **Experimental / repair required.** Source-only audit found speech output-contract, Docker build, API authorization and README discrepancies. Prior live CPU speech evidence exists, but published `main` is not independently verified as runnable. Not production-ready. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local-first camera snapshot archive. A Python watched-folder preview indexes JPEGs, groups frames into visits and serves a browser timeline; a separate refined dashboard uses fictional fixtures. Object detection and vision-model decisions remain future integrations. | **Alpha — synthetic MVP preview.** Published demonstration: 10 fictional JPEGs grouped into 7 visits. No production camera integration or actual model inference demonstrated. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Small Nginx/njs adapter intended to translate Llama Stack model-list and non-streaming chat-completion responses into OpenAI-style JSON. Docker Compose example included; streaming is still a TODO. | **Experimental / legacy prototype.** Source-only review: no published automated tests or verified working deployment; configuration, build, compatibility and security gates remain open. Not production-ready. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Python MCP server that connects clients to Flowise chatflows. Offers FastMCP tools to list chatflows and request predictions, plus low-level dynamic per-chatflow tools. | **Experimental / pre-release.** Source-only review finds tool-authorization, stdio logging, configuration and HTTP error-handling gaps. Not production-ready; assistant integration unverified here. |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** ⭐ 157 | MCP server that dynamically exposes REST APIs described by OpenAPI specs. Dual-stack MCP 1.x / 2.x, with native Streamable HTTP so stateless POST `/mcp` works behind round-robin load balancing without sticky sessions. | **Most mature / release candidate** — package version 0.4.0; CI and the publish workflow are green. Still has 7 open issues, including an unresolved Streamable HTTP `$ref` compatibility bug, and `MCP_ALLOWED_HOSTS` defaults to `*` (protection off). Suitable for evaluation and carefully hardened self-hosting; not a blanket production-ready claim. |
| **[omarchy-deskflow-applet](https://github.com/matthewhand/omarchy-deskflow-applet)** | Omarchy/Quickshell bar applet to control Deskflow client connections and show connection status. Depends on a patched Wayland RemoteDesktop portal. | **Private alpha / not a public release.** Single-system development evidence; clean installation, connection controls and security behaviour are not independently verified. Repository access is restricted. |
| **omarchy-screensaver-cadence** | Fork of Omarchy's screensaver into a rotating ASCII display. A slide list instead of one static file: `text`, `image`, `images DIR`, `exec` and `notify` slides, each with its own dwell time, and slides can pick their own `ttfx` effect and gradient per rotation. | **Private alpha** — the repository is currently private (`omarchy-screensaver-cadence-private`) and works on one machine only. See the honest limits below. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | Flask/Gevent wrapper exposing F5-TTS through OpenAI-style speech and voice/model endpoints, plus optional ElevenLabs-shaped timestamp output with estimated (not forced-aligned) timings. Includes model discovery, audio conversion and a Docker Compose example. | **Experimental / alpha.** Source-only review: README, Docker default voice and verification instructions disagree; runtime inference, API hardening and deployment reliability are unverified. Not production-ready. |

### Why "alpha" and not "beta"

`omarchy-screensaver-cadence` is private alpha because beta would overstate it. It has an
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

## Notes

- This is a curated selection, not a complete inventory. [Browse all public repositories](https://github.com/matthewhand?tab=repositories).
- Some desktop projects remain private, and featured private projects are explicitly labelled.
- "Stable" describes demonstrated maturity; "alpha" and "experimental" indicate unfinished or unverified work.
