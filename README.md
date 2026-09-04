## Hi, I'm sjdhome

I'm a frontend and AI-agent engineer based in Qingdao, China. At work I build browser products with the Fyde & Phi team ([Phi Browser](https://phibrowser.com/), [FydeOS](https://fydeos.io/)). Outside work I make small tools for people who spend their day in a terminal next to an AI coding agent, and I write about how LLMs actually behave.

### What I'm building

- **[Koshell](https://koshell.ai)** ([source](https://github.com/koshell/koshell)) is a human-centric shared terminal. It wraps the shell you already use, turns command boundaries, exit codes and output into structured context an AI can read on demand, and leaves every command under your control. Rust front process, Bun agent daemon, JSONL over a Unix socket. Still early; I write up the design and the negative results as I go.
- **[Teishoku](https://github.com/sjdhome/teishoku)** is a versioned, opinionated menu of engineering decisions that coding agents can read and pin to, so a project does not re-litigate its stack every week.

### Smaller tools

- [tmux-agent-watch](https://github.com/sjdhome/tmux-agent-watch): a read-only TUI that shows whether each AI coding agent in your tmux panes is working, blocked or idle.
- [TmuxAgentWatch](https://github.com/sjdhome/TmuxAgentWatch): the same idea as a native macOS menu bar app.
- [k380-keepalive](https://github.com/sjdhome/k380-keepalive): keeps a flaky Logitech K380 Bluetooth link alive on macOS.

### Writing

- [I instrumented my own product and the data killed my favorite feature](https://koshell.ai/blog/the-data-killed-my-favorite-feature/): 21 days of usage data from Koshell, and why I stopped building the interaction I liked most.
- [LLM 与信息熵](https://sjdhome.com/posts/llm-and-information-entropy/) (Chinese): an LLM is a probability cloud, not a wish-granting machine. Compression, transcription and completion as three ways information flows through it.
- More at [sjdhome.com](https://sjdhome.com), mostly in Chinese.

### How I work

- TypeScript, React and Node / Bun day to day. Rust for the system-level pieces. Python and Go when they fit better.
- I prefer mature abstractions, type safety, tests and graceful degradation over clever code, and I keep a written trail of why decisions were made.
- When something feels wrong, I would rather look at logs and reproduce it than argue from impression.

### Elsewhere

- Website: [sjdhome.com](https://sjdhome.com)
- X: [@sjdhoome](https://x.com/sjdhoome)
