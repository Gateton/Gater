<div align="center">

# Gater
### Serious about code. Never works alone.

A local coding agent that reads your project, plans, runs and verifies.<br>
When the task grows, it calls in a team of specialist kittens.

![Closed source](https://img.shields.io/badge/source-closed-24292f)
![Private beta](https://img.shields.io/badge/status-private_beta-22d3ee)
![Linux first](https://img.shields.io/badge/platform-Linux_first-24292f)
![Windows](https://img.shields.io/badge/platform-Windows-24292f)
![Rust](https://img.shields.io/badge/core-Rust-24292f)

[Watch the video](assets/gater-promo.mp4) · [Explore the product](#everything-it-does-in-plain-sight) · [Request beta access](https://github.com/Gateton/Gater/issues/new?template=beta-access.yml)

[![Watch the Gater promotional video](assets/hero-poster.jpg)](assets/gater-promo.mp4)

</div>

> **Gater is closed-source, built in public.** This repository is its public home for product information, feedback and beta requests. The application source remains private. Gater is in active development; the first stable release is still being prepared.

## Everything it does, in plain sight

Ask for a change in plain language. Gater reads the relevant code, edits files, runs commands and checks the result. Tool activity streams as it happens, changes have inspectable diffs, and `/undo` can revert file changes from the last turn, including the team's work.

Use the terminal TUI or **Gater Desktop**. Both share the same Rust core, sessions, configuration, memory and team.

![Gater Desktop coding workflow](assets/working.webp)

*The Desktop images in this README are design scenarios captured from Gater's actual interface, with example project data. They show the product UI, rather than recorded production sessions.*

### You decide how much freedom it gets

| Mode | How it works |
| --- | --- |
| **Plan** | Reads, asks and proposes a plan before making changes. |
| **Normal** | Asks before commands that change things or write outside the project. |
| **YOLO** | Executes with fewer approval prompts; deleting outside the project still asks. |
| **Turbo** | Takes charge of planning, team coordination and continued verification. |

Keep a persistent plan, follow progress in the Desktop Kanban and steer the task while it runs.

## When the task grows, it calls the team

### Alley · A team built for each task

Gater splits independent work among kittens, gives each a mission, write zone and budget, then integrates and verifies their results. Inspect their activity and conversations, or send a kitten a message while it works.

**Up to 9 helpers per task, with 4 active at once.** These are capacity limits, not default team sizes.

![Alley team workspace](assets/alley.webp)

### Cattery · Your specialists, with memory

Create persistent kittens with their own personality, model, skills and permissions. Their approved memories and work histories carry forward between tasks.

![Cattery specialist profiles](assets/kittens.webp)

| Starter kitten | Specialty |
| --- | --- |
| Scout | Research |
| Razor | Code review |
| Trace | Debugging |
| Probe | Testing |
| Pixel | UI |
| Hiss | Challenging assumptions |

### Rooms · Debate before deciding

Specialists propose independently, critique with evidence and revise their positions. A Room records its outcome, including objections or unresolved questions, so you can continue the discussion with Gater.

![A Grooming review Room](assets/room-grooming.webp)

Built-in modes cover **discussion, research, review, challenge, recovery and exploration**. Room modes can also be customized.

### Attempts · Compare solutions before applying one

Try different implementations in separate copies of the project. Compare changed files, verification results, new dependencies and affected decisions, then choose which attempt to apply.

![Competing implementation attempts](assets/attempts.webp)

## Point at your UI. Gater changes it.

**Workshop** brings a running frontend into Gater Desktop.

1. **Run project:** Gater checks how the app starts and requests permission to run it.
2. **Select:** click the element you want to change.
3. **Ask:** describe the change; Gater locates the relevant code and edits it.
4. **Check:** inspect the updated preview and undo the change if needed.

![Workshop with an element selected](assets/workshop.webp)

## What comes built in

| Capability | What it gives you |
| --- | --- |
| **Approved memory and decisions** | Review what Gater proposes to remember, with reasons and relevant files. |
| **Whole-project checkpoints** | Restore snapshots kept in a separate shadow repository. |
| **Session portability** | Import supported Claude Code, Codex and OpenCode histories without modifying the originals. |
| **Provider choice** | Anthropic, OpenAI and compatible providers such as DeepSeek, OpenRouter and OpenCode Go. API keys or supported subscription authentication. |
| **Usage visibility** | Model, context and available usage information, with estimates distinguished from provider-reported values. |
| **Web and browser tools** | Search documentation, read pages and use browser automation to inspect an app. |
| **Skills and MCP** | Add reusable workflows and tools from explicitly trusted MCP servers. |
| **Images and files** | Attach references and screenshots; vision depends on the selected model or configured vision provider. |
| **18 themes** | Customize the terminal, diffs and pixel cat. |

<details>
<summary>Memory and checkpoints in the Desktop interface</summary>

![A proposed decision for approval](assets/detail-decisions.webp)

![Project checkpoint timeline](assets/detail-checkpoints.webp)

</details>

### A cat that tells you what it is doing

The pixel cat reacts to the agent's state: waiting, thinking, reasoning, working, asking, supervising, errors and sleep. The terminal and Desktop share its identity, and animations can be disabled.

## Beta access

Gater is **Linux first**, with Windows support. Availability and installation instructions will be shared with accepted testers; there is no stable public release yet.

**[Request beta access](https://github.com/Gateton/Gater/issues/new?template=beta-access.yml)** and tell us:

- Your operating system.
- The coding tools and model providers you use.
- A real task you would like to test with Gater.

Requests are public. Do not include API keys, private project files or personal contact details. Requesting access does not guarantee an invitation.

Star or watch this repository for updates. Public builds, when available, will appear in [Releases](https://github.com/Gateton/Gater/releases).

## Feedback and direction

[Report a bug](https://github.com/Gateton/Gater/issues/new?template=bug-report.yml) · [Suggest an improvement](https://github.com/Gateton/Gater/issues/new?template=feature-request.yml)

Current priorities:

- Improve reliability during long coding sessions and team coordination.
- Refine Workshop previews and visual editing.
- Validate provider behavior, usage reporting and session imports.
- Polish Linux and Windows distribution for the first stable release.

These priorities are a direction, not delivery dates.

## FAQ

**Is Gater open source?**  
No. Gater is a proprietary product. This public repository contains presentation materials and community feedback, not the application source. No open-source license is granted for the application.

**Does my code leave my machine?**  
Gater runs locally and stores sessions, memory, decisions and credentials on your computer. Relevant prompts and project content are sent to your selected model provider to perform the task. Web, browser and MCP tools communicate with the services you configure.

**Do I need a model provider?**  
Yes. Bring a supported API key or use subscription authentication where the provider supports it. Model usage is subject to that provider's terms and limits.

**Can I install it now?**  
Request beta access. Builds and supported installation steps are provided as they become available.

## More from the creator

Built by **[Thomas “Gateton” Repka](https://github.com/Gateton)**.

- [pi-usage-live](https://github.com/Gateton/pi-usage-live): provider usage visibility for Pi.
- [session-hub](https://github.com/Gateton/session-hub): tooling for discovering and carrying coding-agent sessions between tools.

---

<div align="center">
Your coding companion. With a whole team of cats.
</div>

