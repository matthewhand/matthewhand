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
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer evolved from OpenAI's experimental Swarm, with Django API, CLI/WebUI, blueprints, handoffs and external-harness adapters. | **Experimental alpha; public CI repair unverified.** | June v0.5.4 predates September source work. Latest public Python run: 8,535 passed, 12 skipped, one asynchronous test race failed on Python 3.13. No public repair PR is available yet. Installation and frontend gates remain open. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python library for hardware/provider detection, shared model-file caching, resource preflight and application status reporting. Applications supply their inference loaders. | **Alpha; 0.3.0 candidate.** | Linux CI and synthetic provider/fixture tests exist. Public installation docs still contain private-development instructions. Versioned publication and real QNN inference are separate verification gates. CPU, DirectML and QNN discovery must remain distinct. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Flask adapter exposing third-party Kokoro speech synthesis through OpenAI-style speech and model-list routes. | **Experimental; draft CPU repair needs corrections.** | Unmerged [PR #3](https://github.com/matthewhand/openai-kokoro-tts/pull/3) has green Python 3.11/3.12 and clean-Docker CI; its report includes real CPU WAV/MP3 synthesis. Independent review reproduced auth-configuration, malformed-input, error-privacy and provider-reporting defects. Human listening, accelerated inference and real-server concurrency remain separate gates. Main has not received this repair. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-JPEG archive and browser visit timeline; separate refined views use fictional fixtures. | **Alpha; synthetic preview, draft hardening.** | Demonstration groups ten fictional JPEGs into seven visits. Unmerged [PR #6](https://github.com/matthewhand/funes-vision/pull/6) has six green CI jobs, including browser and Docker previews. Review found filename-rule drift, an unbounded Node read and incomplete keyboard-reachability proof. Camera ingestion, object detection and vision-model inference remain future work. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for a legacy Llama Stack text-chat/model-list contract and OpenAI-style JSON. | **Experimental legacy prototype; draft repair.** | [Draft PR #1](https://github.com/matthewhand/llama-stack-bridge/pull/1) addresses configuration, container and request-handling problems. No new published verification is available for the follow-up work. Historical request/response compatibility and real nginx/njs execution against a disposable mock upstream remain gates. Streaming and compatibility with current Llama Stack are unproven. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Python MCP connector for Flowise chatflow discovery and predictions, with simple and dynamic tool modes. | **Experimental; draft repair needs corrections.** | Unmerged [PR #8](https://github.com/matthewhand/mcp-flowise/pull/8) has green Python 3.12/3.13 CI and recorded mock/stdio/container proof. Independent review reproduced stale-cache authorization, endpoint-credential leakage and incomplete startup validation. These must be corrected; compatibility with the authenticated live Flowise deployment remains unverified. |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | MCP adapter exposing REST APIs described by OpenAPI specifications, including stdio and Streamable HTTP transports. | **Most established in this selection; compatibility limits remain.** | Package metadata is 0.4.0; current Python CI is green and earlier client/API verification is documented. Streamable HTTP schema issue [#74](https://github.com/matthewhand/mcp-openapi-proxy/issues/74) remains open. Host protection defaults and deployment configuration require an explicit review for the intended environment. |
| **omarchy-deskflow-applet** | Omarchy/Quickshell applet for Deskflow client control and connection status, requiring a patched Wayland RemoteDesktop portal. | **Private alpha.** | Repository access is restricted. Clean installation, connection controls and remote-control consent behavior need a documented verification record. |
| **omarchy-screensaver-cadence** | Rotating ASCII/image/live-data/notification display for Omarchy, with primary/fallback slides, optional bar widget and cached AI text. | **Private alpha; naming and verification tickets open.** | Current repository is named `omarchy-screensaver-cadence-private`; intended name is `omarchy-screensaver-cadence`. The repository documents live demos, but clean installation, idle routing, integrations and current feature claims are being reconciled through issue tickets. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | Flask/Gevent wrapper for F5-TTS speech and voice/model routes, with optional timestamp output using estimated timings. | **Experimental alpha; partial draft hardening.** | [Draft PR #10](https://github.com/matthewhand/openai-f5-tts/pull/10) adds API, path, cache and output safeguards. The follow-up run produced no source changes or new CPU speech proof. Reproducible dependencies, default-model startup, CPU container deployment, privacy and request concurrency remain gates. Estimated timestamps are not forced alignment. Model weights have separate upstream licensing. |

## How to read the status

- **Experimental / alpha:** usable source or a preview exists; important behavior,
  installation or deployment checks remain open.
- **Synthetic verification:** controlled fixtures or mocked dependencies
  demonstrate the tested contract. Hardware and real-service tests have their
  own evidence.
- **Published:** a versioned artifact is available; the source branch and release
  may differ.
- **Private:** featured work is described here, but repository access is restricted.

The linked repair PRs are unmerged candidates, not claims about the current main
branch or a production release. Green CI covers the checks that ran; the remaining
gates above still apply. This profile will be updated as results are integrated.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).

