# claude-plugin (matt-dotfiles marketplace)

A portable, **ADS-agnostic** Claude Code plugin marketplace — the public / air-gapped
counterparts of Matt's internal `matt-plugins` (Azure DevOps) marketplace. Designed to run
on a constrained (Sonnet-4.5 / 200k) orchestrator.

> **Canonical:** Azure DevOps `brain/_git/claude-plugin-external` (private).
> **Public mirror:** `github.com/LDJ-Share/claude-plugin` (this repo). Dual-remote push.
>
> Extracted from `dotfiles/dot-claude` (Epic #388 Phase 3, Story #396), where it had been a
> naive stow package before the proper marketplace mechanism was adopted.

## Install

```sh
/plugin marketplace add LDJ-Share/claude-plugin
/plugin install <name>@matt-dotfiles
```

## Plugins

| Plugin | What it does |
|---|---|
| `orchestrator` | Context-frugal, beads-backed multi-agent orchestrator for a Sonnet-4.5 / 200k window. ADS-agnostic counterpart of `brain-orchestrator`. |
| `dev-workflow` | Trimmed, language-agnostic SDLC (brainstorm → plan → execute → review → finish) + worktrees. Portable counterpart of `superpowers`. |
| `dotnet-style` | Default stack + workflow opinions for modern .NET (C# 12+, NUnit 4, the ReSharper → dotnet format → XAML Styler toolchain). |
| `appium-windows-uia-testing` | Appium UI-automation testing for Windows desktop apps (WPF/WinUI/Win32) over UI Automation. |
| `plugin-self-improvement` | Turns 'aha' moments about the plugins into tracked beads under a self-improvement epic. |

See each plugin's `README.md` for details.
