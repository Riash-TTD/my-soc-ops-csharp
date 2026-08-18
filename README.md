🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

### The Social Bingo game that gets people talking

**Walk up to a stranger. Ask a question. Mark your square. Win bingo.**

[🎮 Play Now](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) &nbsp;·&nbsp; [📚 Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) &nbsp;·&nbsp; [🚀 Get Started](#get-started)

</div>

---

## What is Soc Ops?

Soc Ops is a **Social Bingo** game built for in-person mixers, onboarding events, and team get-togethers. Each square on the 5×5 grid holds an icebreaker question — find a real person who matches it, get their name, and mark it off. First to 5 in a row wins!

Built with **Blazor WebAssembly** on **.NET 10**, it runs entirely in the browser with no backend required.

```
┌─────────────────────────────────────────────┐
│  Has a pet  │ Speaks 3+  │  Ran a 5K  │ ... │
│─────────────│────────────│────────────│─────│
│  Morning    │  Built an  │  Lived     │ ... │
│  person     │  app       │  abroad    │     │
│─────────────│────────────│────────────│─────│
│     ...     │    ...     │   FREE     │ ... │
└─────────────────────────────────────────────┘
         Find people. Start conversations. Win!
```

---

## Get Started

### Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

### Run locally

```bash
cd SocOps
dotnet run
```

Then open [http://localhost:5166](http://localhost:5166) in your browser.

### Open in GitHub Codespaces ☁️

No local setup needed! After creating your own repo from this template:

1. Click **Code** → **Codespaces** → **Create codespace on main**
2. Wait for the devcontainer to finish setup
3. Run `cd SocOps && dotnet run`

### Build

```bash
cd SocOps
dotnet build
```

> Deploys automatically to GitHub Pages on every push to `main`.

---

## 🧪 This is a Copilot Lab

This repo is part of a hands-on workshop for learning **GitHub Copilot agent mode**. You'll build and extend Soc Ops step-by-step, guided by AI.

| Part | What you'll do |
|------|----------------|
| [**00 — Overview**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Understand the project and your goals |
| [**01 — Setup**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configure context engineering for Copilot |
| [**02 — Design**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Build a polished UI with design-first prompts |
| [**03 — Quiz Master**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Create a custom Copilot agent |
| [**04 — Multi-Agent**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Orchestrate multiple agents working together |

> 📝 Lab guides are also available offline in the [`workshop/`](workshop/) folder.
