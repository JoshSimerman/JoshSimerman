### Josh Simerman

I build tooling around AI coding agents: engines that run them safely, ledgers that keep their work
honest, and monitoring that proves it can fire. Most of my work is C# on windows, Python on Linux, and 
TypeScript on Cloudflare.

The repositories below are v1 snapshots exported from private repositories. Each README opens with
a quick start and a few architecture diagrams, and links to deeper docs.

#### Agent tooling

| Project | What it is | Stack |
|---|---|---|
| [atlas-dispatch](https://github.com/JoshSimerman/atlas-dispatch) | Runs AI coding CLIs (Codex, Claude, Gemini, Kimi) in isolated git worktrees, with ref guards, protected paths, failure classification and verified run reports. A demo runs without API keys. | Python, git |
| [atlas-tracker](https://github.com/JoshSimerman/atlas-tracker) | A deliberately small, four-table task ledger for agents. Bad input is refused, never silently dropped. | Python, SQLite, stdlib HTTP |
| [ai-newsletter](https://github.com/JoshSimerman/ai-newsletter) | Sift: a daily AI news digest. Parallel Claude Code agents do the research, and a deterministic renderer and scripted gates decide what gets published. | Node.js, Cloudflare Pages, D1 |

#### Reliability and data

| Project | What it is | Stack |
|---|---|---|
| [honest-watchdogs](https://github.com/JoshSimerman/honest-watchdogs) | Monitoring tools that prove they can fire: positive controls for launchd and systemd watchers, mount probes, guarded mirrors and alert delivery. | Python, macOS, Linux |
| [regime-engine](https://github.com/JoshSimerman/regime-engine) | A Bitcoin market-cycle classifier: on-chain data harvesting, pillar scoring and a hysteresis state machine. It ships example thresholds only. | Python, PostgreSQL |

#### Apps and setup

| Project | What it is | Stack |
|---|---|---|
| [notes-app](https://github.com/JoshSimerman/notes-app) | A single-user notes app you deploy to your own domain: sign-in with Cloudflare Access, nightly backups, scheduled cleanup. | TypeScript, React, Cloudflare Workers, D1, R2 |
| [omarchy-setup](https://github.com/JoshSimerman/omarchy-setup) | An Omarchy (Arch Linux and Hyprland) workstation built by directing AI coding agents, with a change log and an audit trail of every decision. | Bash, Arch Linux |
