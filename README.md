# homebrew-agenthandover

Homebrew tap for [AgentHandover](https://github.com/sandroandric/AgentHandover) — a local, privacy-first workflow apprentice that turns your laptop work into AI-executable SOPs.

## Install

```bash
brew tap sandroandric/agenthandover
brew install --cask agenthandover
```

This installs the signed, notarized `.pkg` from the [AgentHandover releases page](https://github.com/sandroandric/AgentHandover/releases). You get bit-identical behavior to the direct-download install path, so all TCC (Accessibility + Screen Recording), launchd, and Ollama onboarding flows work the same.

## Uninstall

```bash
brew uninstall --cask agenthandover
```

To also wipe data and preferences (`~/Library/Application Support/agenthandover`, launch agents, caches):

```bash
brew uninstall --zap --cask agenthandover
```

## What this tap ships

- `Casks/agenthandover.rb` — cask that downloads the latest signed `.pkg`.

The source of truth for the cask lives at `homebrew/Casks/agenthandover.rb` in the main [AgentHandover repo](https://github.com/sandroandric/AgentHandover); this tap is a one-file mirror.
