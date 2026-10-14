# Hey, I'm matthewh

I work on a personal [Omarchy](https://omarchy.dev) desktop and the tooling around
it — an AI-assisted setup where agent tooling, window-manager configuration and
the desktop itself are all first-class citizens.

I publish small tools, experiments and substantial derivative work. This is a
curated selection, with upstream origins acknowledged where applicable.

## Projects

Status and evidence reviewed **14 October 2026**. A published version, passing
tests and a demonstration each establish different things. The table records
the evidence available for each project and the remaining verification.

| Project | What it does | Current status | Evidence and remaining work |
|---|---|---|---|
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer evolved from OpenAI's experimental Swarm, with Django API, CLI/WebUI, blueprints, handoffs and external-harness adapters. | **Experimental alpha; CI repair in progress.** | June v0.5.4 predates September source work. Latest public Python run: 8,535 passed, 12 skipped, one asynchronous test race failed on Python 3.13. The focused fix exists in private development and is being verified for the public source. Installation and frontend gates are being rechecked. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python library for hardware/provider detection, shared model-file caching, resource preflight and application status reporting. Applications supply their inference loaders. | **Alpha; 0.3.0 candidate.** | Linux CI and synthetic provider/fixture tests exist. Public installation docs still contain private-development instructions. Versioned publication and real QNN inference are separate verification gates. CPU, DirectML and QNN discovery must remain distinct. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Flask adapter exposing third-party Kokoro speech synthesis through OpenAI-style speech and model-list routes. | **Experimental; repair branch under verification.** | Published main has inconsistent Docker/Python requirements and incompatible handler/audio-output contracts. An existing CPU-hardening branch addresses these; clean Docker build, real WAV/MP3 synthesis, model/voice compatibility and optional provider work are being verified before integration. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-JPEG archive and browser visit timeline; separate refined views use fictional fixtures. | **Alpha; synthetic preview.** | Demonstration groups ten fictional JPEGs into seven visits. An unmerged hardening branch is being tested for file handling, browser behavior and installation. Camera ingestion, object detection and vision-model inference remain future work. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for a legacy Llama Stack text-chat/model-list contract and OpenAI-style JSON. | **Experimental legacy prototype; draft repair.** | Draft PR #1 addresses configuration, container and request-handling problems. Historical request/response compatibility and real nginx/njs execution against a disposable mock upstream are being verified. Streaming and compatibility with current Llama Stack are unproven. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Python MCP connector for Flowise chatflow discovery and predictions, with simple and dynamic tool modes. | **Experimental; repair in progress.** | Source review found dispatch/filter gaps, protocol-stdout logging, ambiguous HTTP failures and Docker/Python inconsistency. Both-mode stdio integration, reproducible packaging and actual Flowise compatibility are verification gates. |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | MCP adapter exposing REST APIs described by OpenAPI specifications, including stdio and Streamable HTTP transports. | **Most established in this selection; compatibility limits remain.** | Package metadata is 0.4.0; current Python CI is green and earlier client/API verification is documented. Streamable HTTP schema issue [#74](https://github.com/matthewhand/mcp-openapi-proxy/issues/74) remains open. Host protection defaults and deployment configuration require an explicit review for the intended environment. |
| **omarchy-deskflow-applet** | Omarchy/Quickshell applet for Deskflow client control and connection status, requiring a patched Wayland RemoteDesktop portal. | **Private alpha.** | Repository access is restricted. Clean installation, connection controls and remote-control consent behavior need a documented verification record. |
| **omarchy-screensaver-cadence** | Rotating ASCII/image/live-data/notification display for Omarchy, with primary/fallback slides, optional bar widget and cached AI text. | **Private alpha; naming and verification tickets open.** | Current repository is named `omarchy-screensaver-cadence-private`; intended name is `omarchy-screensaver-cadence`. The repository documents live demos, but clean installation, idle routing, integrations and current feature claims are being reconciled through issue tickets. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | Flask/Gevent wrapper for F5-TTS speech and voice/model routes, with optional timestamp output using estimated timings. | **Experimental alpha; draft repair under verification.** | Draft PR #10 adds API, path, cache and output safeguards. Reproducible dependencies, default-model startup, CPU container deployment, request concurrency and actual synthesized audio are being tested. Estimated timestamps are not forced alignment. Model weights have separate upstream licensing. |

## How to read the status

- **Experimental / alpha:** usable source or a preview exists; important behavior,
  installation or deployment checks remain open.
- **Synthetic verification:** controlled fixtures or mocked dependencies
  demonstrate the tested contract. Hardware and real-service tests have their
  own evidence.
- **Published:** a versioned artifact is available; the source branch and release
  may differ.
- **Private:** featured work is described here, but repository access is restricted.

Repair work stays on candidate branches until review and verification are complete.
This profile will be updated as those results are integrated.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
