# Agentometer

Agentometer is a free Mac beta that puts agent usage limits, RAM, and storage in a desktop widget. Open the menu bar app to see more details, including CPU and battery readings.

The universal download requires macOS 14 or later and includes Apple silicon and Intel binaries. Runtime testing covered Apple silicon. Intel runtime testing is pending.

## Install

1. Download `Agentometer-0.1.12-beta-macos-universal.zip`. [0.1.12 beta release](https://github.com/chf-NewStart/Agentometer/releases/tag/v0.1.12)
2. Unzip the download and drag `Agentometer.app` into **Applications**.
3. Open Agentometer. Right-click the desktop, choose **Edit Widgets**, and add the medium Agentometer widget for the combined overview.
4. To start Agentometer when you sign in, enable **Launch at login** in its options menu.

## Connect your agents

The integrations are optional. Agentometer shows the session and weekly limits each provider makes available, along with their reset times. The letter marks CX, CL, and H identify Codex, Claude, and Hermes.

- **Codex** uses an existing, signed-in Codex CLI installation.
- **Claude** uses an existing Claude Code installation. Connect it in Agentometer, then use Claude Code to receive a reading. The bundled native bridge runs without Python.
- **Hermes** connects to a dashboard with the Ollama usage plugin. The readings reflect the configured Ollama account’s limits.

## Privacy

Agentometer caches readings and settings on your Mac. Provider requests go through your configured integrations, and Hermes credentials are stored in macOS Keychain. Agentometer sends no telemetry to the developer.

This repository hosts documentation and release downloads for the independent Agentometer app. [Releases](https://github.com/chf-NewStart/Agentometer/releases)
