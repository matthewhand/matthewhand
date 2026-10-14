# Hey, I'm matthewh

I work on a personal [Omarchy](https://omarchy.dev) desktop and the tooling around it — an AI-assisted setup where agent tooling, window-manager configuration and the desktop itself are all first-class citizens.

I publish small tools, experiments and substantial derivative work, with upstream origins acknowledged where applicable. This is a curated selection, not a claim that every project is production-ready.

## Projects

**Public-source status checked 15 October 2026.** “Working demonstration”, “implemented source”, “draft change” and “publicly released” mean different things. Descriptions refer to the linked **public repository** unless stated otherwise.

| Project | What it does | Evidence-based status |
|---|---|---|
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent operating layer with WebUI, CLI, API, handoffs and integrations with external agent harnesses. | **Experimental, actively developed source.** The public README includes walkthroughs and architecture, but a documented demonstration is not a guarantee of a clean install, current CI status or general production readiness. |
| **[snapdragon-npu-hexagon-kit](https://github.com/matthewhand/snapdragon-npu-hexagon-kit)** | Python hardware/provider discovery, model-cache and resource-preflight library; applications provide their own inference loaders. | **Alpha source; 0.3.0 candidate.** Provider discovery and synthetic checks do not prove actual Hexagon/QNN inference or a published 0.3.0 package. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Flask API adapter for Kokoro text-to-speech, including OpenAI-style speech routes. | **Experimental implementation.** [Draft PR #3](https://github.com/matthewhand/openai-kokoro-tts/pull/3) is still unmerged; candidate-branch CPU synthesis evidence does not establish equivalent behavior on public main or every target system. |
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Browses JPEGs added to a local watched folder and groups successive images into a visit timeline; offers synthetic interface previews. | **Working public watched-folder and visit-browser demonstration, not a released camera-analysis system.** The public Python-server proof shows **10 fictional JPEGs grouped into 7 visits**. Example object labels come from **synthetic metadata**, not executed YOLO, System1 or a vision LLM. The public main README does not establish live-camera ingestion, deployed object detection or decision-model inference. [Draft PR #6](https://github.com/matthewhand/funes-vision/pull/6) remains unmerged; private or draft work is not presented as a public release. |
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs request-and-response adapter for a legacy Llama Stack chat API. | **Experimental legacy prototype.** [Draft PR #1](https://github.com/matthewhand/llama-stack-bridge/pull/1) is unmerged; compatibility with today's Llama Stack and live streaming has not been verified here. |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | MCP server exposing Flowise chatflows and predictions in simple or dynamic tool modes. | **Experimental connector.** [Draft PR #8](https://github.com/matthewhand/mcp-flowise/pull/8) is unmerged. Mock and source-level checks must not be confused with a verified live authenticated Flowise deployment. |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | Exposes OpenAPI-described REST endpoints as MCP tools, using stdio or Streamable HTTP. | **Versioned 0.4.0 source with documented compatibility tests.** Actual security and client compatibility depend on deployment and protocol versions; [Streamable HTTP issue #74](https://github.com/matthewhand/mcp-openapi-proxy/issues/74) is documented. |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | Flask/Gevent speech API wrapper around F5-TTS, including customizable voice selection. | **Historically used application; current reproducibility not independently re-tested for this profile.** [Draft PR #10](https://github.com/matthewhand/openai-f5-tts/pull/10) contains documentation, security and reliability work but is still unmerged. Earlier synthetic regression results do not constitute fresh model synthesis, container deployment or concurrency proof. Estimated timestamps are not forced alignment. |

Other private Omarchy experiments include a Deskflow control applet and a cadence-style screensaver. They are **private, not independently reproducible public releases**; their presence here should not be read as an installation or feature-support promise.

## Reading these statuses

A **synthetic demo** proves only the exercised fixture workflow. **Source in a draft pull request** is not a feature released on main. **Historical successful use** does not mean a fresh test was performed today. A public README describes intended and documented behavior, while hardware, model-inference and production claims require their own evidence.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
