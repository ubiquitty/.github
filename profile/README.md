<!-- Copyright (C) 2026 Stanislav Yaglo -->
<!-- SPDX-License-Identifier: Apache-2.0 -->

# Ubiquitty

**A terminal for people and agents. Native apps, polished terminal views, and a portable engine with a persistent multiplexer.**

[Get the apps](https://github.com/ubiquitty/ubiquitty#install) · [Embed a terminal view](https://github.com/ubiquitty/ubiquitty-kit) · [Build with Core](https://github.com/ubiquitty/ubiquitty-core)

<a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/opencode-proportional.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/opencode-proportional.png" width="1000" alt="A native Ubiquitty window connected to a Linux host: OpenCode answers in proportional text beside a deployment dashboard, with an attached-agent badge in the title bar."></a>

*OpenCode with Ubiquitty's rich-text integration: readable prose beside aligned code and a live terminal dashboard.*

### Work that stays with you

The host owns the running processes, terminal state, and scrollback. Disconnect a client and reattach to the same session; open it from the native Mac app or a browser, with each client drawing its own view.

`ubq` brings CLI and MCP access to that same live terminal. Agents can read the screen, send input, and wait for changes. The host enforces permissions and asks for human consent when an agent requests access to an occupied session. MCP tools cannot approve themselves. [Remote sessions and agents →](https://github.com/ubiquitty/ubiquitty/blob/main/Docs/guides/remote-sessions-and-agents.md)

### Typography worth looking at

Proportional rich text alongside terminal programs, careful shaping and ligatures, color emoji, styled underlines, and inline graphics. The macOS app pairs CoreText with Metal; the reusable renderers and native views live in UbiquittyKit.

<p>
  <a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/polish.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/polish.png" width="440" alt="Terminal typography showing five underline styles, superscripts and subscripts, and mathematical expressions with joined brackets."></a>
  <a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/web-shared-session.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/web-shared-session.png" width="440" alt="Safari and the native Mac app displaying the same Neovim buffer in a session on the Linux host hub."></a>
</p>

*Fine typography in the terminal; one host-owned Neovim session shared by browser and native clients.*

### Choose your starting point

| You want to… | Start here |
|---|---|
| Use the terminal apps and persistent multiplexer | [**Ubiquitty apps**](https://github.com/ubiquitty/ubiquitty) — macOS, iOS, Linux, and web frontends. [Install or build →](https://github.com/ubiquitty/ubiquitty#install) |
| Add a performant, polished terminal view to your app | [**UbiquittyKit**](https://github.com/ubiquitty/ubiquitty-kit) — finely tuned typography; Metal views for macOS and iOS; Vulkan, FreeType, and software renderers for Linux. [Native-view API →](https://github.com/ubiquitty/ubiquitty-kit/blob/main/Docs/ubiquittykit-api.md) |
| Own the UI, embed the engine, or build on persistent sessions | [**Ubiquitty Core**](https://github.com/ubiquitty/ubiquitty-core) — C++/C terminal engine, `libubiquitty`, `ubiquitty-host`, Sync, and CLI/MCP access with host-enforced permissions. [Embedding guide →](https://github.com/ubiquitty/ubiquitty-core/blob/main/Docs/libubiquittycore.md) |

**4,529 / 4,529 applicable conformance cases passed (100%).** Ubiquitty was also the **fastest parser among the engines and workloads in our comparative runs**. These are suite and parser-throughput results; rendering, latency, and energy are measured separately. [Conformance scope](https://github.com/ubiquitty/ubiquitty#conformance) · [Benchmark methods](https://github.com/ubiquitty/ubiquitty#benchmarks)

> The multiplexer and remote sessions are experimental. The Linux GTK app currently supports local sessions, without host attach. See the [platform and build guide](https://github.com/ubiquitty/ubiquitty/blob/main/Docs/platform-builds.md) for the status of each frontend.

Apache-2.0 open source. [Contribute](https://github.com/ubiquitty/ubiquitty/blob/main/.github/contributing.md) · [Ubiquitty.org](https://ubiquitty.org)
