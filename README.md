<div align="center">

<img src="assets/social-preview.png" alt="Gater: your coding companion, with a whole team of cats" width="720">

<br>

### Serious about code. Never works alone.

A local coding agent that reads your project, plans, runs and verifies.<br>
When the task grows, it calls in a team of specialist kittens.

<br>

![Closed source](https://img.shields.io/badge/source-closed-24292f)
![Private beta](https://img.shields.io/badge/status-private_beta-22d3ee)
![Linux first](https://img.shields.io/badge/platform-Linux_first-24292f)
![Windows](https://img.shields.io/badge/platform-Windows-24292f)
![Rust](https://img.shields.io/badge/core-Rust-24292f)
![Terminal and desktop](https://img.shields.io/badge/interface-TUI_%2B_Desktop-24292f)

**[See it in motion](#see-it-in-motion)** ·
**[In the terminal](#in-the-terminal)** ·
**[Meet the team](#when-the-task-grows-it-calls-the-team)** ·
**[Request beta access](https://github.com/Gateton/Gater/issues/new?template=beta-access.yml)**

[English](README.md) · [Español](README.es.md)

</div>

> **Gater is closed-source, built in public.** This repository is its public home for product information, feedback and beta requests. The application source remains private. Gater is in active development; the first stable release is still being prepared.

<br>

## See it in motion

A two-minute tour of the terminal, the desktop app, the team, Rooms, Workshop, checkpoints and themes.

https://github.com/user-attachments/assets/a452abb6-cef1-4f9c-b9bd-84255028dabf

<div align="center">

<sub>Prefer a file? <a href="assets/gater-promo.mp4?raw=true">Download the tour</a> (MP4, 720p, 7.7 MB)</sub>

</div>

<br>

## Gater at a glance

<div align="center">

| | | | |
| :---: | :---: | :---: | :---: |
| **2**<br>interfaces, one core<br><sub>terminal and desktop</sub> | **4**<br>work modes<br><sub>Plan, Normal, YOLO, Turbo</sub> | **9**<br>helpers per task<br><sub>4 working at once</sub> | **6**<br>kittens included<br><sub>and you can make more</sub> |
| **6**<br>Room modes<br><sub>to debate before deciding</sub> | **2–3**<br>competing attempts<br><sub>compared on evidence</sub> | **18**<br>themes<br><sub>terminal, diffs and cat</sub> | **5**<br>agent histories<br>you can import<br><sub>originals stay untouched</sub> |

</div>

<br>

## What Gater can do

Ask for a change in plain language. Gater reads the relevant code, edits files, runs commands and checks the result. Tool activity streams as it happens, changes have inspectable diffs, and `/undo` can revert file changes from the last turn, including the team's work.

Gater lives in two places: your **terminal** and **Gater Desktop**. Both share the same Rust core, sessions, configuration, memory and team, so what you start in one you can continue in the other.

### In the terminal

The terminal UI is where Gater started, and it is a full citizen: streaming reasoning and tool calls, a side panel for the plan, the team and the files that changed, the whole alley, permissions, memory and themes. No window needed.

![Gater in the terminal: reasoning, tool calls and test results streaming live, with the queue and the changed files in the side panel](assets/tui-working.webp)


<table>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/tui-alley.webp" alt="The Agents tab with four kittens working in parallel: Luna, Simba, Michi and Nala"><br>
      <b>The alley, in the side panel</b><br>
      Four kittens working in parallel, each with its zone, status, tokens and cost.
    </td>
    <td width="50%" valign="top">
      <img src="assets/tui-plan.webp" alt="A plan waiting for approval, with the alley's cats assigned to each step"><br>
      <b>Plans you approve</b><br>
      Review the steps, see who takes each one and choose YOLO or Turbo.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/tui-permission.webp" alt="A permission request for running cargo test, with approve, always and reject"><br>
      <b>Permissions you can read</b><br>
      Approve once, remember a command for the project, or say no.
    </td>
    <td width="50%" valign="top">
      <img src="assets/tui-cat-room.webp" alt="Michi's room: its mission, its steps and the report it handed back"><br>
      <b>Step into any cat's room</b><br>
      Read exactly what a kitten did, and write to it while it works.
    </td>
  </tr>
</table>

<details>
<summary><b>More of the terminal</b>: team board, themes, memory and session import</summary>

<br>

![The team board: zones, agreements and what each kitten posted](assets/tui-board.webp)

![The theme picker with live preview: the whole interface already wears the tabby theme](assets/tui-themes.webp)

![Light theme in the terminal](assets/tui-light.webp)

![Memory notes waiting for approval](assets/tui-memory.webp)

![Importing sessions from Pi, Claude Code, Codex, OpenCode and Jcode](assets/tui-sessions.webp)

</details>

### On the desktop

**Gater Desktop** puts the same agent in a window: a Kanban for the plan, the alley's stage, Rooms, Workshop and checkpoints as visual views.

![Gater Desktop coding workflow](assets/working.webp)

*The terminal images in this README are rendered straight from Gater's real terminal UI with example project data. The Desktop images are design scenarios captured from Gater's actual interface, also with example project data. Neither shows a recorded production session.*

### How a task flows

1. **You describe it.** In plain language, with screenshots or files attached if that helps.
2. **Gater looks first.** It reads and searches your project, and proposes a plan when the task deserves one.
3. **It works in the open.** Every read, edit and command streams live, and every changed file has a diff.
4. **It verifies.** It runs your tests and checks before it calls the work done.
5. **You stay in control.** Steer it mid-turn, `/undo` the whole turn, or restore a project checkpoint.

### You decide how much freedom it gets

| Mode | How it works |
| --- | --- |
| **Plan** | Reads, asks and proposes a plan before making changes. Nothing changes until you approve it. |
| **Normal** | Asks before commands that change things or write outside the project. |
| **YOLO** | Executes with fewer approval prompts; deleting outside the project still asks. |
| **Turbo** | Takes charge of planning, team coordination and continued verification until it is done and verified. |

Switch modes with `Shift+Tab`. Keep a persistent plan, follow progress in the Desktop **Kanban**, and steer the task while it runs: `Enter` folds a new instruction into the current turn, `Shift+Enter` queues it for later.

<br>

## When the task grows, it calls the team

### Alley · A team built for each task

Gater splits independent work among kittens, gives each a mission, write zone and budget, then integrates and verifies their results. Inspect their activity and conversations, or send a kitten a message while it works.

**Up to 9 helpers per task, with 4 active at once.** These are capacity limits, not default team sizes.

![Alley team workspace](assets/alley.webp)


### Cattery · Your specialists, with memory

Create persistent kittens with their own personality, model, skills and permissions. Their approved memories and work histories carry forward between tasks. Save a group of them as a **clowder** and bring it back whenever you need it.

![Cattery specialist profiles](assets/kittens.webp)

| Starter kitten | Specialty | What it does |
| --- | --- | --- |
| **Scout** | Research | Answers by reading code, docs and the web, with a source for every claim. |
| **Razor** | Code review | Hunts for real bugs and missing cases, and verifies each finding. |
| **Trace** | Debugging | Reproduces, forms hypotheses, isolates, fixes the cause and leaves a regression test. |
| **Probe** | Testing | Writes and runs tests that fail for the right reason. |
| **Pixel** | UI | Reviews running interfaces: states, contrast, narrow windows, keyboard use. |
| **Hiss** | Challenging assumptions | Looks for the weakest assumption, the forgotten case and the cheaper alternative. |

### Rooms · Debate before deciding

Specialists propose independently, critique with evidence and revise their positions. A Room records its outcome, including objections or unresolved questions, so you can continue the discussion with Gater.

![A Grooming review Room](assets/room-grooming.webp)


| Room mode | Use it to |
| --- | --- |
| **Caterwaul** · Discussion | Gather blind proposals, critique with citations, then revise to a final position. |
| **Prowl** · Research | Split a question, investigate each part with sources and consolidate. |
| **Grooming** · Review | Review from several angles blind, then cross-verify the findings. |
| **Scratch** · Challenge | Attack a design or code with evidence, running commands in a copy. |
| **Landing** · Recovery | Work from evidence to cause to a proposed fix after something broke. |
| **Nine Lives** · Exploration | Develop a different alternative per kitten, then compare and recommend. |

Room modes are plain files, so you can customize them or write your own.

### Attempts · Compare solutions before applying one

Try different implementations in separate copies of the project. Compare changed files, verification results, new dependencies and affected decisions, then choose which attempt to apply.

![Competing implementation attempts](assets/attempts.webp)

<br>

## Point at your UI. Gater changes it.

**Workshop** brings a running frontend into Gater Desktop.

1. **Run project:** Gater checks how the app starts and requests permission to run it.
2. **Select:** click the element you want to change.
3. **Ask:** describe the change; Gater locates the relevant code and edits it.
4. **Check:** inspect the updated preview and undo the change if needed.

![Workshop with an element selected](assets/workshop.webp)


<br>

## A cat that tells you what it is doing

The pixel cat reacts to the agent's state, in the terminal and on the desktop. The animations can be turned off with `/animations off`.

![The eight states of the Gater cat: waiting, thinking, reasoning, working, asking, supervising, on alert and asleep](assets/cat-states.png)

<br>

## You stay in control

| Capability | What it gives you |
| --- | --- |
| **Approved memory and decisions** | Gater proposes what to remember and which decisions to keep, with reasons and relevant files. Nothing is saved without your say-so, and it warns you when a change contradicts a decision. |
| **Whole-project checkpoints** | Restore snapshots kept in a separate shadow repository, outside your own. Taken automatically before big changes. |
| **`/undo`** | Reverts the file changes of the last turn, including what the team did. |
| **Permissions you can read** | Approve a call once, or remember a command pattern for the project, and revoke it later from settings. |
| **Project journal** | A running diary of where the project stands, what comes next and what is broken. |

<details>
<summary>Memory and checkpoints in the Desktop interface</summary>

![A proposed decision for approval](assets/detail-decisions.webp)

![Project checkpoint timeline](assets/detail-checkpoints.webp)

</details>

<br>

## What comes built in

| Capability | What it gives you |
| --- | --- |
| **Provider choice** | Anthropic, OpenAI and compatible providers such as DeepSeek, OpenRouter and OpenCode Go. API keys or supported subscription authentication. |
| **Usage visibility** | Model, context and available usage information, with estimates distinguished from provider-reported values. |
| **Web and browser tools** | Search documentation, read pages as Markdown and use browser automation to inspect an app. |
| **Skills and hooks** | Reusable workflows in `SKILL.md` format (review, security review, debug, write tests, commit and PR, UI check and more), plus hooks that run around tool calls and turns. |
| **MCP** | Add tools from MCP servers you explicitly trust, trimmed per server and per kitten. |
| **Session portability** | Import supported Claude Code, Codex, OpenCode, jcode and pi histories without modifying the originals. |
| **Branch a conversation** | `/btw` asks a side question without losing the main thread. |
| **Images and files** | Attach references and screenshots; vision depends on the selected model or configured vision provider. |
| **Context you can see** | A live context meter and `/compact` to condense a long session. |
| **18 themes** | Customize the terminal, diffs and pixel cat, with live preview. Dark and light, from the quiet cyan of `gater-dark` to `tabby`, `neon-alley` and `porcelain`. |
| **Accessibility** | Keyboard-first, screen-reader friendly, reduced-motion aware, with contrast checked across all 18 themes in Desktop. |

<details>
<summary>Slash command quick reference</summary>

| Area | Commands |
| --- | --- |
| **Work** | `/plan` `/mode` `/yolo` `/turbo` `/undo` `/cancel` `/compact` `/bash` `/cd` |
| **Team** | `/alley` `/kittens` `/rooms` |
| **Context** | `/memory` `/checkpoints` `/journal` `/skills` `/mcp` |
| **Sessions** | `/sessions` `/new` `/rename` `/delete` `/resume` `/btw` `/debug` |
| **Models** | `/login` `/logout` `/models` `/thinking` `/usage` `/vision` `/connections` |
| **Look and feel** | `/themes` `/animations` `/panel` |
| **Other** | `/config` `/help` `/quit` |

From the command line: `gater` opens the terminal UI, `gater desktop` opens the app, and `gater run "…"` runs a single turn without an interface, which is handy in scripts.

</details>

<br>

## Beta access

Gater is **Linux first**, with Windows support. Availability and installation instructions will be shared with accepted testers; there is no stable public release yet.

**[Request beta access](https://github.com/Gateton/Gater/issues/new?template=beta-access.yml)** and tell us:

- Your operating system.
- The coding tools and model providers you use.
- A real task you would like to test with Gater.

Requests are public. Do not include API keys, private project files or personal contact details. Requesting access does not guarantee an invitation.

Star or watch this repository for updates. Public builds, when available, will appear in [Releases](https://github.com/Gateton/Gater/releases).

<br>

## Feedback and direction

[Report a bug](https://github.com/Gateton/Gater/issues/new?template=bug-report.yml) · [Suggest an improvement](https://github.com/Gateton/Gater/issues/new?template=feature-request.yml)

Current priorities:

- Improve reliability during long coding sessions and team coordination.
- Refine Workshop previews and visual editing.
- Validate provider behavior, usage reporting and session imports.
- Polish Linux and Windows distribution for the first stable release.

These priorities are a direction, not delivery dates.

<br>

## FAQ

<details>
<summary><strong>Is Gater open source?</strong></summary>

No. Gater is a proprietary product. This public repository contains presentation materials and community feedback, not the application source. No open-source license is granted for the application.

</details>

<details>
<summary><strong>Does my code leave my machine?</strong></summary>

Gater runs locally and stores sessions, memory, decisions and credentials on your computer. Relevant prompts and project content are sent to your selected model provider to perform the task. Web, browser and MCP tools communicate with the services you configure.

</details>

<details>
<summary><strong>Do I need a model provider?</strong></summary>

Yes. Bring a supported API key or use subscription authentication where the provider supports it. Model usage is subject to that provider's terms and limits.

</details>

<details>
<summary><strong>Can I undo what it does?</strong></summary>

Yes. `/undo` reverts the file changes of the last turn, including the team's work, and project checkpoints let you go back to earlier moments without touching your own repository. In Normal mode, commands that change things ask first.

</details>

<details>
<summary><strong>Can I use it from the terminal only?</strong></summary>

Yes. The terminal UI and Gater Desktop share the same core, so you can use either one, or switch between them mid-project. Workshop, the Kanban plan and the visual team views are Desktop features.

</details>

<details>
<summary><strong>Can I install it now?</strong></summary>

Request beta access. Builds and supported installation steps are provided as they become available.

</details>

<br>

## More from the creator

Built by **[Thomas “Gateton” Repka](https://github.com/Gateton)**.

- [pi-usage-live](https://github.com/Gateton/pi-usage-live): provider usage visibility for Pi.
- [session-hub](https://github.com/Gateton/session-hub): tooling for discovering and carrying coding-agent sessions between tools.

---

<div align="center">
Your coding companion. With a whole team of cats.
</div>
