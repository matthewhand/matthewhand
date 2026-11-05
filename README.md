# Hey, I'm matthewh

I build local-first AI tools, agent workflows and useful apps, spanning speech, vision, automation and hardware integration.

My projects and integrations come first in each category. Forks are labelled with their upstream projects.

## Embodied AI & Interactive Systems

| Project | Description |
|---|---|
| **[open-wiimote](https://github.com/matthewhand/open-wiimote)** | Wii Remote buttons and tilt as a virtual gamepad, with desktop and browser interfaces. **Linux x64 prerelease** · [ISC](https://github.com/matthewhand/open-wiimote/blob/main/LICENSE) · [Downloads](https://github.com/matthewhand/open-wiimote/releases) · [Roadmap](https://github.com/matthewhand/open-wiimote#roadmap).<br><br><img src="https://raw.githubusercontent.com/matthewhand/open-wiimote/main/docs/images/open-wiimote.svg" alt="OpenWiimote: bring your Wii Remote back into play" width="400" height="100"> |
| **[openai-f5-tts](https://github.com/matthewhand/openai-f5-tts)** | Independent [F5-TTS](https://github.com/SWivid/F5-TTS) API wrapper for self-hosted speech, selectable voices, custom checkpoints, sentence-level PCM streaming and estimated timestamps. **Community beta** · [MIT](https://github.com/matthewhand/openai-f5-tts/blob/main/LICENSE) wrapper; pretrained model weights are separately CC-BY-NC. |
| **[openai-kokoro-tts](https://github.com/matthewhand/openai-kokoro-tts)** | Independent, CPU-first OpenAI-compatible speech API around [Kokoro](https://huggingface.co/hexgrad/Kokoro-82M) and [kokoro-onnx](https://github.com/thewh1teagle/kokoro-onnx). **Community beta** · [MIT](https://github.com/matthewhand/openai-kokoro-tts/blob/main/LICENSE) wrapper; Kokoro-82M weights are Apache-2.0. |
| [audio.cpp-hub](https://github.com/matthewhand/audio.cpp-hub) | Web management for audio.cpp instances and speech/audio tasks. Fork of [IIIIIllllIIIIIlllll/audio.cpp-hub](https://github.com/IIIIIllllIIIIIlllll/audio.cpp-hub). |
| [GroqCasters](https://github.com/matthewhand/GroqCasters) | AI podcast generation, with F5-TTS added alongside Bark. Fork of [jgravelle/GroqCasters](https://github.com/jgravelle/GroqCasters). |
| [labs-Voice-Agent](https://github.com/matthewhand/labs-Voice-Agent) | Voice-agent framework. Fork of [NVIDIA-NeMo/labs-Voice-Agent](https://github.com/NVIDIA-NeMo/labs-Voice-Agent). |
| [talkbot](https://github.com/matthewhand/talkbot) | Discord speech and translation bot. Fork of [nullabork/talkbot](https://github.com/nullabork/talkbot). |
| [ugv_rpi](https://github.com/matthewhand/ugv_rpi) | Waveshare Raspberry Pi UGV software. Fork of [waveshareteam/ugv_rpi](https://github.com/waveshareteam/ugv_rpi). |
| [VoiceMem](https://github.com/matthewhand/VoiceMem) | Streaming memory for voice agents. Fork of [xzf-thu/VoiceMem](https://github.com/xzf-thu/VoiceMem). |
| [webxr-samples](https://github.com/matthewhand/webxr-samples) | WebXR browser examples. Fork of [immersive-web/webxr-samples](https://github.com/immersive-web/webxr-samples). |

OpenWiimote targets Windows and macOS too; macOS virtual-gamepad output is not implemented. The speech wrappers are independent of OpenAI and the upstream model authors.

## Cross-Platform Desktop Experiences

| Project | Description |
|---|---|
| **[waltop-osx](https://github.com/matthewhand/waltop-osx)** | Userspace pen-pressure support for the WALTOP Slim Tablet 12.1 on macOS. **Hardware integration** · [MIT](https://github.com/matthewhand/waltop-osx/blob/main/LICENSE). |
| [omarchy-chronos](https://github.com/matthewhand/omarchy-chronos) | Omarchy clock and calendar. Fork of [nixfred/omarchy-chronos](https://github.com/nixfred/omarchy-chronos). |
| [omarchy-osk](https://github.com/matthewhand/omarchy-osk) | Omarchy on-screen keyboard. Fork of [ekollof/omarchy-osk](https://github.com/ekollof/omarchy-osk). **Archived.** |
| [OpenMausBot](https://github.com/matthewhand/OpenMausBot) | Desktop coordination for Claude/Codex agents. Fork of [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot). |
| [persona](https://github.com/matthewhand/persona) | Desktop avatar reacting to voice output from other apps. Fork of [xikhar/persona](https://github.com/xikhar/persona). |
| [rift](https://github.com/matthewhand/rift) | Omarchy workspace app placement. Fork of [nixfred/rift](https://github.com/nixfred/rift). |

## Edge AI & Hardware Acceleration

| Project | Description |
|---|---|
| [amd-strix-halo-image-video-distrobox](https://github.com/matthewhand/amd-strix-halo-image-video-distrobox) | ROCm image/video containers for AMD Strix Halo. Fork of [kyuz0/amd-strix-halo-image-video-toolboxes](https://github.com/kyuz0/amd-strix-halo-image-video-toolboxes). **Archived.** |
| [chatterbox](https://github.com/matthewhand/chatterbox) | AMD adaptation of the Chatterbox Pinokio launcher. Fork of [Deathdadev/chatterbox](https://github.com/Deathdadev/chatterbox). |
| [ChatterCraft-Pinokio](https://github.com/matthewhand/ChatterCraft-Pinokio) | AMD launcher adaptation for storytelling and voice cloning. Fork of [TheAwaken1/ChatterCraft-Pinokio](https://github.com/TheAwaken1/ChatterCraft-Pinokio). |
| [Chattered](https://github.com/matthewhand/Chattered) | AMD launcher adaptation for a Chatterbox Gradio interface. Fork of [6Morpheus6/Chattered](https://github.com/6Morpheus6/Chattered). |
| [MagicQuill](https://github.com/matthewhand/MagicQuill) | AMD launcher adaptation for interactive image editing. Fork of [pinokiofactory/MagicQuill](https://github.com/pinokiofactory/MagicQuill). |
| [openaudio](https://github.com/matthewhand/openaudio) | AMD launcher adaptation for Fish Speech/OpenAudio. Fork of [pinokiofactory/openaudio](https://github.com/pinokiofactory/openaudio). |
| [Orpheus-TTS-FastAPI](https://github.com/matthewhand/Orpheus-TTS-FastAPI) | AMD launcher adaptation for an Orpheus speech API. Fork of [pinokiofactory/Orpheus-TTS-FastAPI](https://github.com/pinokiofactory/Orpheus-TTS-FastAPI). |
| [Ultimate-TTS-Studio](https://github.com/matthewhand/Ultimate-TTS-Studio) | AMD launcher adaptation for multi-engine speech. Fork of [pinokiofactory/Ultimate-TTS-Studio](https://github.com/pinokiofactory/Ultimate-TTS-Studio). |
| [vibevoice-realtime](https://github.com/matthewhand/vibevoice-realtime) | AMD launcher adaptation for VibeVoice realtime speech. Fork of [pinokiofactory/vibevoice-realtime](https://github.com/pinokiofactory/vibevoice-realtime). |

AMD-focused container and launcher adaptations; application and accelerator support varies by repository.

## Smart Home & Intelligent Automation

| Project | Description |
|---|---|
| **[funes-vision](https://github.com/matthewhand/funes-vision)** | Local watched-folder browser for JPEG snapshots and grouped visits, with a demo gallery. **Public alpha** · [MIT](https://github.com/matthewhand/funes-vision/blob/main/LICENSE). |
| [holman-linux-python](https://github.com/matthewhand/holman-linux-python) | Holman irrigation SDK for Python/Linux. Fork of [scottmckenzie/holman-linux-python](https://github.com/scottmckenzie/holman-linux-python). |
| [htpc-download-box](https://github.com/matthewhand/htpc-download-box) | Docker media and Plex stack. Fork of [sebgl/htpc-download-box](https://github.com/sebgl/htpc-download-box). |
| [InkMemories](https://github.com/matthewhand/InkMemories) | Connected eInk photo frame. Fork of [tymzd/InkMemories](https://github.com/tymzd/InkMemories). |

## AI Infrastructure & Developer Tools

| Project | Description |
|---|---|
| **[llama-stack-bridge](https://github.com/matthewhand/llama-stack-bridge)** | Nginx/njs adapter for Llama Stack model lists and non-streaming chat. **Legacy prototype** · [MIT](https://github.com/matthewhand/llama-stack-bridge/blob/main/LICENSE). |
| **[mcp-flowise](https://github.com/matthewhand/mcp-flowise)** | Discover and run Flowise chatflows from MCP clients, with authentication and flow filtering. **Experimental** · [MIT](https://github.com/matthewhand/mcp-flowise/blob/main/LICENSE). |
| **[mcp-openapi-proxy](https://github.com/matthewhand/mcp-openapi-proxy)** | OpenAPI-described REST APIs as MCP tools over Streamable HTTP or stdio. **Versioned tool** · [MIT](https://github.com/matthewhand/mcp-openapi-proxy/blob/main/LICENSE) · [Docs](https://github.com/matthewhand/mcp-openapi-proxy#readme) · [Releases](https://github.com/matthewhand/mcp-openapi-proxy/releases). |
| **[operating-swarm](https://github.com/matthewhand/operating-swarm)** | Agent workflows across model APIs, agent CLIs and remote harnesses, with a shared API, CLI and WebUI. Evolved from [OpenAI Swarm](https://github.com/openai/swarm). **Experimental alpha** · [MIT](https://github.com/matthewhand/operating-swarm/blob/main/LICENSE). |
| [open-webui-integrations](https://github.com/matthewhand/open-webui-integrations) | Open WebUI functions for routing, Flowise, reasoning, consensus, AutoGen and image generation. Integration collection; attribution in the source headers. |
| [perplexica-aws](https://github.com/matthewhand/perplexica-aws) | AWS deployment scripts and configuration for a Perplexica-based search system. |
| [accept-a-payment](https://github.com/matthewhand/accept-a-payment) | Stripe payment examples. Fork of [stripe-samples/accept-a-payment](https://github.com/stripe-samples/accept-a-payment). |
| [ansible_role_microk8s](https://github.com/matthewhand/ansible_role_microk8s) | MicroK8s deployment on Ubuntu. Fork of [istvano/ansible_role_microk8s](https://github.com/istvano/ansible_role_microk8s). |
| [docker-compose-ui](https://github.com/matthewhand/docker-compose-ui) | Docker Compose management interface. Fork of [francescou/docker-compose-ui](https://github.com/francescou/docker-compose-ui). |
| [herdr](https://github.com/matthewhand/herdr) | Coding-agent runtime. Fork of [herdrdev/herdr](https://github.com/herdrdev/herdr). |
| [omniplex](https://github.com/matthewhand/omniplex) | AI search application. Fork of [Omniplex-ai/omniplex](https://github.com/Omniplex-ai/omniplex). |
| [open-webui](https://github.com/matthewhand/open-webui) | Local and hosted LLM interface. Fork of [open-webui/open-webui](https://github.com/open-webui/open-webui). |
| [openmuse-1](https://github.com/matthewhand/openmuse-1) | Personal agent with browser, terminal and files. Fork of [CopilotKit/openmuse](https://github.com/CopilotKit/openmuse). |
| [openwebui-docs](https://github.com/matthewhand/openwebui-docs) | Open WebUI documentation. Fork of [open-webui/docs](https://github.com/open-webui/docs). |
| [rakazo](https://github.com/matthewhand/rakazo) | Multi-agent assistant. Fork of [elie222/rakazo](https://github.com/elie222/rakazo). |
| [self-hosted-ai-starter-kit](https://github.com/matthewhand/self-hosted-ai-starter-kit) | Docker-based local AI starter stack. Fork of [n8n-io/self-hosted-ai-starter-kit](https://github.com/n8n-io/self-hosted-ai-starter-kit). |
| [server-wp-mcp](https://github.com/matthewhand/server-wp-mcp) | WordPress MCP server; configuration, packaging and test additions. Fork of [emzimmer/server-wp-mcp](https://github.com/emzimmer/server-wp-mcp). |
| [stripe-checkout-next-js-demo](https://github.com/matthewhand/stripe-checkout-next-js-demo) | Next.js/Stripe checkout example. Fork of [projectashik/stripe-checkout-next-js-demo](https://github.com/projectashik/stripe-checkout-next-js-demo). |
| [trueforge](https://github.com/matthewhand/trueforge) | Agent harness. Fork of [truefoundry/trueforge](https://github.com/truefoundry/trueforge). |
| [vectara-ingest](https://github.com/matthewhand/vectara-ingest) | Crawlers and ingestion pipelines. Fork of [vectara/vectara-ingest](https://github.com/vectara/vectara-ingest). |

**Supporting repositories:** [matthewhand](https://github.com/matthewhand/matthewhand) (this profile) · [matthewhand.github.io](https://github.com/matthewhand/matthewhand.github.io) (personal website source).

See each repository and its upstream documentation for current setup, platform support and limitations. Models, dependencies and assets retain their own licence terms.

[Browse all public repositories](https://github.com/matthewhand?tab=repositories).
