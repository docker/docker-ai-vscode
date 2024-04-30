# Docker VSCode Limited Early Access
As mentioned in the release notes, the `.vsix` file described here provides early access to features that
we are proposing to be contributed into the official Docker vscode extension.

## Dependencies
These updates require a local [Docker Desktop](https://www.docker.com/products/docker-desktop/) and a running
docker engine.

## Installation

### Step 1: Download Extension File
Two VSCode extensions are available:
- Dockerfile Language Features: https://github.com/docker/docker-vscode/releases/tag/lsp-v1.29.5-alpha
- Generate runnable makefile in markdown: https://github.com/docker/docker-vscode/releases/tag/runbook-v0.0.2

Download the `.vsix` bundle.

### Step 2: Enable Extension in VSCode

#### CLI:

Must have VSCode [code](https://code.visualstudio.com/docs/editor/command-line#_code-is-not-recognized-as-an-internal-or-external-command) command in PATH:

```bash
code --install-extension /my/path/to/docker-bundle.vsix --force
```

#### GUI:

Extensions -> `...` menu -> `Install from VSIX`

<img width="570" alt="Screenshot of docker install menu" src="https://github.com/docker/docker-ai/assets/5000430/1cf2b904-f341-4a84-aceb-1933c51efe68">

#### GUI (command palette):

1. Type `>` into top search bar
**Shortcut: Press ⇧⌘P (OSX) or CTRL⇧P (Win/Linux)**
2. Select `Extensions: Install from VSIX...`
3. Select `.vsix` file downloaded
4. Hit the “Reload Now” button in the notification at the bottom right corner

## Usage
Open a Dockerfile to get diagnostics
