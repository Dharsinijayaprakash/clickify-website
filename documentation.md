# Clickify ✦ Photo Studio — Documentation

> **Your moment, perfectly framed.**  
> A 100% private, browser-based photo booth studio. No servers. No uploads. No tracking.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Getting Started](#getting-started)
   - [Creating an Account](#creating-an-account)
   - [Signing In](#signing-in)
4. [Studio](#studio)
   - [Camera Setup](#camera-setup)
   - [Capture Modes](#capture-modes)
   - [Filters](#filters)
   - [Frames](#frames)
   - [Stickers](#stickers)
   - [Settings](#settings)
5. [Gallery](#gallery)
6. [Privacy & Data Storage](#privacy--data-storage)
7. [Tech Stack](#tech-stack)
8. [Deployment](#deployment)
9. [License](#license)

---

## Overview

**Clickify** is a private, in-browser photo studio that lets users take photos using their device's camera, apply filters, frames, and stickers, and save them — all locally on their device. No photos are ever uploaded to any server.

- 🌐 **Live App:** [clickifybooth.vercel.app](https://clickifybooth.vercel.app)
- 👤 **Author:** Dharshini Jayaprakash
- 📅 **Year:** 2025

---

## Features

| Feature | Description |
|---|---|
| 🔒 Private Accounts | Multi-user support with separate, isolated photo galleries per account |
| 📷 Live Camera Feed | Real-time camera preview inside the browser |
| 🎞️ Multiple Capture Modes | Single shot, Strip ×4, and Burst ×3 |
| 🎨 Filters | Apply photo filters (e.g., Natural) to your shots |
| 🖼️ Frames | Decorate photos with decorative frames |
| ✨ Stickers | Overlay emoji/sticker overlays on photos (❤️, 🌸, ⭐, 🦋, 🎀, 👑, 🦄, and more) |
| 🗃️ Local Gallery | Browse, download, and delete saved photos |
| 🎞️ Film Strip Export | Download all shots as a film strip |
| 📵 No Uploads | Everything stays on the user's browser/device |
| 🛡️ No Tracking | No analytics, no email required |

---

## Getting Started

### Creating an Account

1. Visit [clickifybooth.vercel.app](https://clickifybooth.vercel.app).
2. Click **"Don't have an account? Create one free"**.
3. Fill in the following fields:
   - **Username** *(required)* — Your unique login name.
   - **Display Name** *(optional)* — A friendly name shown in the studio.
   - **Password** *(required)* — Choose a secure password.
   - **Confirm Password** *(required)* — Re-enter your password.
4. Click **"Create Account →"**.

> ℹ️ No email address is required. All account data is stored locally in your browser.

---

### Signing In

1. On the landing page, enter your **Username** and **Password**.
2. Click **"Sign In →"**.
3. You will be taken to your personal **Studio** dashboard.

> ⚠️ Since all data is stored on the browser, clearing browser storage/cookies will erase your account and photos.

---

## Studio

The Studio is the main workspace where you capture photos.

### Camera Setup

On first use, Clickify will request camera permission from your browser.

**To enable the camera:**
1. Click **"Enable Camera"**.
2. If the browser blocks it, locate the 🔒 lock icon in the address bar.
3. Click it and set **Camera** to **"Allow"**.
4. Reload the page and tap **Enable Camera** again.

> 📌 The camera is automatically turned off when the browser tab is closed.

---

### Capture Modes

Choose from three capture modes before shooting:

| Mode | Description |
|---|---|
| **Single** | Takes one photo per click |
| **Strip ×4** | Takes 4 sequential photos in a film strip layout |
| **Burst ×3** | Rapidly captures 3 photos in a burst |

The current frame count is shown as `0 / N` on the capture button.

---

### Filters

Click **🎨 Filters** to apply a filter to your photos before or during capture.

Available filters include:
- ☀️ Natural (default)
- *(Additional filters may be available via the in-app menu)*

---

### Frames

Click **🖼️ Frames** to wrap your photo in a decorative border/frame.

Frames can be selected from the frame picker panel that slides in from the toolbar.

---

### Stickers

Click **✨ Stickers** to overlay an emoji sticker onto your photo.

Available stickers:
`❤️` `✨` `🌸` `⭐` `🔥` `🦋` `🌈` `🎀` `💫` `🍀` `🌙` `🎵` `🌺` `👑` `🦄`

---

### Settings

Click **⚙️ Settings** to adjust:
- **Photo Size** — Resolution of captured photos (default: `1280×960`)
- Additional preferences as available in the panel

---

## Gallery

The **Gallery** tab shows all photos saved during your sessions.

### Actions

| Action | Description |
|---|---|
| **⬇ Download** | Save a single photo to your device |
| **↓ Strip** | Download all photos as a film strip |
| **↓ All** | Download all individual photos |
| **🗑 Delete** | Remove a single photo |
| **🗑 Clear All** | Remove all photos from the gallery |

> 📌 Photos show metadata like ISO and shot count (e.g., `ISO 400 · Saved 0 shots`).

Gallery is private per account — other users on the same device cannot view your photos.

---

## Privacy & Data Storage

Clickify is designed with **privacy-first** principles:

- ✅ All photos are stored **only on your device** (browser `localStorage` or `IndexedDB`).
- ✅ Each user account's photos are stored **separately**.
- ✅ **No data is ever sent to a server.**
- ✅ **No analytics or tracking** of any kind.
- ✅ No email or personal information required to register.
- ✅ Camera access is released when the tab is closed.

> ⚠️ Because storage is browser-local, uninstalling the browser, clearing site data, or using a different browser/device will result in loss of photos and account data.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Camera API | Web `getUserMedia` / `MediaStream` API |
| Storage | Browser LocalStorage / IndexedDB |
| Hosting | [Vercel](https://vercel.com) |
| Source | [GitHub Pages mirror](https://dharsinijayaprakash.github.io/clickify-website/) |

---

## Deployment

The app is deployed on **Vercel** and accessible at:

```
https://clickifybooth.vercel.app
```

A GitHub Pages mirror is also available at:

```
https://dharsinijayaprakash.github.io/clickify-website/
```

To run locally (if you have the source):
```bash
# No build step required — open index.html directly in a browser
open index.html
```

Or serve with a simple local server:
```bash
npx serve .
# Then visit http://localhost:3000
```

---

## License

© 2025 Clickify · Made with 💕 by Dharshini Jayaprakash  
*Your memories, your device.*

---

*This documentation was generated based on the live application at [clickifybooth.vercel.app](https://clickifybooth.vercel.app).*
