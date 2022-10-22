---
title: Installer
blurb: A GUI installer and troubleshooter for BetterDiscord, built in Electron and Svelte.
icon: installer.png
repo: BetterDiscord/Installer
layout: project.njk
---

# Installer

<img src="/assets/projects/images/installer.webp" alt="BetterDiscord Installer" />


## What is this?

This repository contains the source code for the BetterDiscord installer. This installer is written with [electron-webpack](https://webpack.electron.build/) and [Svelte 3](https://svelte.dev/).

## Codebase

```
.
├──assets                  // Contains static assets (such as images) used by the installer.
|  └──images               // Images (logos, backgrounds, etc...) used by the installer.
├──scripts                 // Scripts needed for development and contributing.
└──src                     // The installer's source code.
    ├──main                // Electron "main" process. Creates and configures the BrowserWindow.
    └──renderer            // Electron "renderer" process. Contains most components and scripts.
        ├──actions         // Scripts performed by the installer such as installing, repairing and uninstalling.
        |  └──utils        // Common utilities used by installer actions (such as killing discord).
        ├──common          // Common UI components such as buttons, checkboxes, radios, etc...
        ├──pages           // Component files for each page in the installer's setup process.
        ├──stores          // Svelte store used for storing global data.
        |  └──types        // Used for defining custom svelte stores.
        └──transitions     // Contains custom Svelte transitions and animations.