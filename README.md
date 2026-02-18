# 🎀 Ribbon Collector — User Guide

Welcome, ribbon collector!  
This site is designed to feel like an NPC interaction in a game. Use the dialog choices to explore ribbons, plan meetups, and track your collection during the convention.

---

## 📱 How to Use the Site

Everything works through the **dialog box choices** on the screen.  
Just tap a selection to continue the conversation.

You can always use:
- ⬅️ **Back** — return to the previous screen
- 🏠 **Ribbon Menu** — go back to ribbon browsing

---

## 🎀 Browsing Ribbons

From the ribbon menu, you can choose how to explore:

### 🏷️ Show me a dealers list
Displays all dealers offering ribbons.

Tap a dealer to:
- View all ribbons they offer
- Tap a ribbon image to open details

---

### 🎨 Show me a fandom list
Displays ribbons grouped by fandom.

Tap a fandom to:
- See related ribbons
- Open details for any ribbon

---

### 🎀 Show me a list of all ribbons
Displays every ribbon in a scrollable list.

You can:
- Tap an image to view details
- See tracking badges (🟡 Want / ✅ Got)

---

## ⭐ Ribbon Detail Screen

When you open a ribbon, you can:

- View:
  - Dealer
  - Fandom
  - How to earn
  - Days available

### 🟡 Status Tracking
You can mark ribbons to help track your progress:

Tap: Status: Not tracking → Want 🟡 → Got ✅ → Not tracking


This is saved **only on your device**.

Badges appear on ribbon images:
- 🟡 Want — you're hunting this ribbon
- ✅ Got — you collected it

---

## 📅 Events & Meetups

The Events menu lists ribbon-related meetups.

From here you can:
- View time, day, and location

---

## 📤 Sharing the App

Use the **Share** option to send the site to another collector.

On phones, this opens the native share menu:
- Text message
- Email
- Discord
- Other apps

A QR code is also shown for quick scanning.

---

## 💬 About & Discussion

You may find options to:
- Open the community Discord
- Learn about the Ribbon Game
- Submit new ribbons

These open external pages in a new tab.

---

# 🔒 Privacy & Data Storage

Your privacy matters. This site is designed to work **without accounts or tracking**. This does not include any external sites, like Discord or Google Forms.

## What is stored locally
If you use ribbon status tracking, the site saves:
- Which ribbons you marked as Want 🟡 or Got ✅

This is stored using your browser’s local storage.

## Important notes
- Data stays **only on your device**
- Nothing is uploaded to a server
- No personal information is collected
- Clearing your browser data will erase your ribbon tracking

## Cookies
This site does **not** use tracking cookies, ads, or analytics cookies.

---

# Developers

A phone-first, single-page web app that feels like an NPC dialog menu.  
It lets congoers browse ribbons by **Dealer**, **Fandom**, or **All**, tap a ribbon image to view details.

This project is designed to be easy to maintain with minimal coding:

- Update ribbon data in `Config/Ribbons.csv`
- Drop ribbon images into `Config/ImageRibbons/`
- Update meetup data in `Config/Meetups.csv`

This project can be customized for a convention by updating

- Update Information in `Config/app_config.json`
- Update Background Image at `Config/imageBackground.png`
- Update QR Code Image at `Config/imageQRcode.png`

**Advanced** Update NPC's Conversation's Path

- Update the `Config/Conversations.json`

---

## Live Site (GitHub Pages)

After publishing, your site will be available at:

- `https://<YOUR_GITHUB_USERNAME>.github.io/<REPO_NAME>/`

Example:

- `https://shinryoku31.github.io/ConRibbons/`

---

## GitHub Pages Setup

### Option A (Recommended): Deploy from `main` branch root

1. Go to your repo on GitHub
2. Click **Settings**
3. Click **Pages**
4. Under **Build and deployment**
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Click **Save**
6. Wait for GitHub Pages to publish (refresh the Pages section to see the live URL)

### Option B: Deploy from `/docs` folder

If you prefer the `/docs` pattern:

1. Move `index.html` and `Config/` into `/docs`
2. In **Settings → Pages**
   - Branch: `main`
   - Folder: `/docs`

> Only use one approach. The project expects paths like `./Config/...` relative to `index.html`.
