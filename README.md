# Llama Farm

Llama Farm turns the computers, old phones and tablets you already own into a small AI farm on your home network.
Your coding agents (Claude Code, Codex CLI, Gemini CLI) hand quick jobs to the farm instead of spending tokens on
them: summarizing files, filtering build logs, looking up code, drafting commit messages. The models run on your own
devices, so that work never leaves your network.

> **This is an alpha.** Expect rough edges, and please tell us when you hit one (see [Report a problem](#report-a-problem)).

This repository only hosts the builds. The source code isn't published.

## Download

Get the newest build from **[Releases](../../releases)**. Under **Assets**, pick the file for your computer:

| Computer | File | Needs |
|----------|------|-------|
| Mac | `Llama Farm-<version>.dmg` | Apple silicon (M1 or later), macOS 14 or later |
| Windows | `Llama Farm-<version>.msi` | Windows 10 or 11, 64-bit |
| Linux | `llama-farm_<version>-1_amd64.deb` | Ubuntu, Debian or another `.deb` distribution, 64-bit |

**Android phones and tablets** get Llama Farm from Google Play's testing track. Ask for an invite, and once you're
added, the Play Store link installs it and keeps it up to date.

## Install

- **Mac:** open the `.dmg` and drag **Llama Farm** into **Applications**.
- **Windows:** run the `.msi`. Windows may say it "protected your PC" because the alpha isn't signed yet: choose
  **More info**, then **Run anyway**.
- **Linux:** `sudo apt install ./llama-farm_<version>-1_amd64.deb`

On first launch, Llama Farm asks what this device should be. The computer you code on is usually the **farm**.
Every other device joins it as a **node**: on the farm, choose **Settings → Add node**; on the device, open Llama
Farm, choose **Node**, and scan or type the code the farm shows. Then choose
**Connect AI tools** on the farm to set up your coding agents.

## Updates

When a new build is out, the desktop app shows **Update** in its header and in **Settings → About**. Download the new
build and install it over the old one; your farm and settings stay. On Android, Play updates the app for you.

## Report a problem

In the app, go to **Settings → About → Report a problem**. It opens an email with the version, your device and the
app's recent log already filled in, with secrets hidden. Add what happened, then send it.

If the app won't open, email **stingersolutionsdev@gmail.com** with your version and your OS. The desktop log is at
`~/.llama-fleet/logs/app.log` (on Windows, `%USERPROFILE%\.llama-fleet\logs\app.log`).

## Privacy

Everything runs on your devices and your network. Llama Farm collects no data and has no account. It goes online for
three things only:
- downloading the models you pick;
- checking this page for new builds;
- if you choose Orchestrator mode, calling the AI provider you set up, with your own API key.
