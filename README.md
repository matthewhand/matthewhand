# Hey, I'm matthewh

I work on a personal [Omarchy](https://omarchy.dev) desktop and the tooling around
it — an AI-assisted setup where the agent tooling, the window manager config and
the desktop itself are all first-class citizens.

Most of what I publish is small and specific. The maturity column is meant
honestly: I'd rather label something **alpha** than imply it's finished.

## Built from scratch

| Project | What it does | Maturity |
|---|---|---|
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
| `holman-linux-python` | `scottmckenzie/holman-linux-python` — **no longer public** | Kept as a local fork and deliberately never pushed back. The upstream repo has since disappeared, so no patch can be diffed or credited. | **Local only.** I didn't trust an AI-assisted workflow not to push unfinished work upstream, so it stayed here. |

I also carry private mirrors of several upstream projects I use on the desktop
(an `xdg-desktop-portal-hyprland` fork with `RemoteDesktop` support, plus a
Deskflow source mirror), kept private so I can patch them without upstream noise.

## Notes

- The bar widgets I wrote for my own desktop live in private repos, except
  `omarchy-screensaver-cadence`.
- Anything labelled stable above is something I'd use again tomorrow. Anything
  labelled alpha is a work in progress that happens to be public.