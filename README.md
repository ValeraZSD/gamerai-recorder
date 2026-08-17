# GamerAI Recorder — downloads

This repository exists only to host downloads. There is no source code here.

**[Download the latest version](../../releases/latest)**

## What this is

A small Windows app that records Scrap Mechanic gameplay — the game window
only — so it can be used to train an AI to play the game. If somebody sent you
here, they are collecting that footage.

- It records **only the Scrap Mechanic window**: never your desktop, never
  other windows, never a second monitor.
- The picture is saved small: 192×192 for training, plus a 720p copy you can
  watch back.
- It **pauses when you alt-tab away**, so nothing outside the game is captured.
- Your microphone is recorded only if you switch that on yourself.
- Nothing is uploaded automatically. You press a button to package your
  recordings, and you choose whether to send the file.

The app asks for all of this once, in plain language, the first time you run
it, in one of ten languages.

## Installing

1. Download the `.zip` from [the latest release](../../releases/latest).
2. Unzip it anywhere you like — **not** into `Program Files`; a normal folder
   such as your Desktop or Documents works best, because that is what lets the
   app update itself later.
3. Run `GamerAI-Recorder.exe`. There is nothing to install.

Windows SmartScreen may warn you that the app is unrecognised: it is not
code-signed. Choose *More info* → *Run anyway* if you trust whoever sent you
here.

## Updating

The app checks this page for itself when it starts. When there is a newer
version it shows a notice saying which version you are on and which one is
available — for example *1.1.1 → 1.2.0* — and, if you have skipped a few, how
many releases behind you are.

The notice has two buttons: **Update now** downloads and installs the new
version and restarts the app, and **What changed** opens the
[releases page](../../releases) so you can read what each version you missed
actually changed.

You can carry on recording and update later — the notice will still be there
next time. It cannot be dismissed, because an old recorder can quietly go on
producing footage that a fixed bug has already made less useful.

## The files in each release

| file | what it is |
|---|---|
| `GamerAI-Recorder-<version>.zip` | the app |
| `version.json` | the manifest the app reads to see whether it is out of date |

`version.json` carries the SHA-256 of the zip, so the app can check its
download arrived intact. It also lists every release published so far, which
is how the app can tell you how many versions you have skipped without having
to ask GitHub anything else.

## Problems

The app has a **Something went wrong** button that writes a report file
containing logs and settings — no gameplay. Send that to whoever gave you the
recorder.
