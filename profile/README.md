<!-- Copyright (C) 2026 Stanislav Yaglo -->
<!-- SPDX-License-Identifier: Apache-2.0 -->

# Ubiquitty

**A terminal and multiplexer you can share with your agents.**

[Get the apps](https://github.com/ubiquitty/ubiquitty#install) · [Embed a terminal view](https://github.com/ubiquitty/kit) · [Build with Core](https://github.com/ubiquitty/core)

**100% conformance: 4,532 / 4,532 applicable cases passed, versus about 66% for the next-best tested engine in our recorded comparison.**

**The fastest parser in our comparative benchmarks, as of 7 November 2026.** [Conformance scope](https://github.com/ubiquitty/ubiquitty#conformance) · [Benchmark methods](https://github.com/ubiquitty/ubiquitty#benchmarks)

<sub>libghostty-vt main (cf3a8a659) scored 66.3% in our tests on 12 November 2026. Parser throughput, rendering, latency, and energy are measured separately.</sub>

<a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/opencode-proportional.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/opencode-proportional.png" width="1000" alt="A native Ubiquitty window connected to a Linux host: OpenCode answers in proportional text beside a deployment dashboard, with an attached-agent badge in the title bar."></a>

*OpenCode with Ubiquitty's rich-text integration: readable prose beside aligned code and a live terminal dashboard.*

### Work that stays with you

The host owns the running processes, terminal state, and scrollback. Disconnect a client and reattach to the same session; open it from the native Mac app or a browser, with each client drawing its own view.

`ubq` brings CLI and MCP access to that same live terminal. Agents can read the screen, send input, and wait for changes. The host enforces permissions and asks for human consent when an agent requests access to an occupied session. MCP tools cannot approve themselves. [Remote sessions and agents →](https://github.com/ubiquitty/ubiquitty/blob/main/Docs/guides/remote-sessions-and-agents.md)

### Terminal compatibility

Legacy terminal software renders correctly, including double-height text,
national character sets, protected cells and DEC rectangular screen editing.

Kitty keyboard input, animated Kitty graphics, Sixel, iTerm2 images, OSC 8 links
and synchronized output are supported by the same engine. The most conformant
engine in our recorded comparison powers the apps and the libraries.

Extended DECPS adds eight musical channels, waveform voices, WAV samples,
envelopes, filters, reverb and tracker effects. Programs can use it for
instruments, sequencers and game audio; the Mac app supplies playback.
[Sound protocol](https://ubiquitty.org/features/sound/).

### Typography worth looking at

Proportional rich text alongside terminal programs, careful shaping and ligatures, color emoji, styled underlines, and inline graphics. The macOS app pairs CoreText with Metal; the reusable renderers and native views live in UbiquittyKit.

<p>
  <a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/polish.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/polish.png" width="440" alt="Terminal typography showing five underline styles, superscripts and subscripts, and mathematical expressions with joined brackets."></a>
  <a href="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/web-shared-session.png"><img src="https://raw.githubusercontent.com/ubiquitty/ubiquitty/main/Docs/images/web-shared-session.png" width="440" alt="Safari and the native Mac app displaying the same Neovim buffer in a session on the Linux host hub."></a>
</p>

*Fine typography in the terminal; one host-owned Neovim session shared by browser and native clients.*

Beam reaches commands, settings, command blocks and scrollback from one palette.
Copy a command’s output, keep its formatting, paste shell-escaped text and find
recent copies in the paste panel. Program-reported status shows which tab is
working, done or waiting for you.

### Choose your starting point

| You want to… | Start here |
|---|---|
| Use the terminal apps and persistent multiplexer | [**Ubiquitty apps**](https://github.com/ubiquitty/ubiquitty) — macOS, iOS, Linux, and web frontends. [Install or build →](https://github.com/ubiquitty/ubiquitty#install) |
| Add a performant, polished terminal view to your app | [**UbiquittyKit**](https://github.com/ubiquitty/kit) — finely tuned typography; Metal views for macOS and iOS; Vulkan, FreeType, and software renderers for Linux. [Native-view API →](https://github.com/ubiquitty/kit/blob/main/Docs/ubiquittykit-api.md) |
| Own the UI, embed the engine, or build on persistent sessions | [**Ubiquitty Core**](https://github.com/ubiquitty/core) — portable terminal engine, `libubiquitty`, `ubiquitty-host`, Sync, and CLI/MCP access with host-enforced permissions. [Embedding guide →](https://github.com/ubiquitty/core/blob/main/Docs/libubiquittycore.md) |

> The multiplexer and remote sessions are experimental. The Linux GTK app currently supports local sessions, without host attach. See the [platform and build guide](https://github.com/ubiquitty/ubiquitty/blob/main/Docs/platform-builds.md) for the status of each frontend.

Apache-2.0 open source. [Contribute](https://github.com/ubiquitty/ubiquitty/blob/main/.github/contributing.md) · [Ubiquitty.org](https://ubiquitty.org)
