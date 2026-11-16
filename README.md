## Hi, I'm sjdhome

I'm a frontend and AI-agent engineer based in Qingdao, China. At work I build browser products with the Fyde & Phi team ([Phi Browser](https://phibrowser.com/), [FydeOS](https://fydeos.io/)). Outside work, when something on my own machines misbehaves, I follow it down the stack until I can name the cause, send a fix or a reproducible report upstream, and write up how I got there.

### Sent upstream

- **wlroots** ([!5483](https://gitlab.freedesktop.org/wlroots/wlroots/-/merge_requests/5483)): Sway could not light up any display after a long suspend. wlroots kept a stale CRTC assignment across suspend, so the kernel rejected every atomic commit after resume. The patch re-reads each connector's CRTC from the kernel when the session resumes.
- **AeroSpace** ([pull requests](https://github.com/nikitabobko/AeroSpace/pulls?q=is%3Apr+author%3Asjdhome)): a series of focus fixes for the macOS tiling window manager, such as focus jumping after a click on another monitor and the MRU order getting lost when closed windows are restored. I run a build with these patches every day.
- **Chromium** ([issue 586203821](https://issues.chromium.org/issues/586203821)): on Wayland, a tiled window that gets `window.resizeTo` or CDP `Browser.setWindowBounds` paints at the requested size in a corner of its tile and leaves the rest black. Found while testing my own upstream build under Sway.
- **pi-subagents** ([#458](https://github.com/tintinweb/pi-subagents/issues/458)): `inherit_context` drops tool results and cannot reuse the parent's prompt cache. I proposed a `fork` agent type that continues the parent session instead of summarizing it, and I run one locally.

### Writing

Mostly debugging write-ups, in Chinese, at [sjdhome.com](https://sjdhome.com):

- [Sway 睡眠唤醒后双屏黑屏：wlroots 记错了 CRTC](https://sjdhome.com/posts/wlroots-stale-crtc-after-suspend/): the investigation behind the wlroots patch, wrong turns included.
- [macOS 27 上 tmux 里 ssh 报 Undefined error: 0](https://sjdhome.com/posts/macos-tmux-ssh-undefined-error-0/): an error code that says nothing, traced to the local network permission of a terminal process that no longer exists.
- [在 Mac 上用 UTM 直通 USB 硬盘跑 Ubuntu Server，并让 TRIM 生效](https://sjdhome.com/posts/utm-usb-passthrough-ubuntu-trim/) and [its cold-boot follow-up](https://sjdhome.com/posts/utm-usb-boot-disk-cold-start/): running a VM straight off an external NVMe drive with the USB passthrough added in macOS 27.

### How I work

- TypeScript, React and Node / Bun day to day. Rust for system-level pieces, and I read C and C++ when the problem lives lower in the stack.
- When something feels wrong, I would rather read the logs and reproduce it than argue from impression.
- I work with AI coding agents every day, and my write-ups say which parts were mine and which were the agent's.
- I prefer mature abstractions, type safety, tests and graceful degradation over clever code, and I keep a written trail of why decisions were made.

### Elsewhere

- Website: [sjdhome.com](https://sjdhome.com)
- X: [@sjdhoome](https://x.com/sjdhoome)
