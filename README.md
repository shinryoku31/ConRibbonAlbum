# ConRibbonsAlbums 🎀 (NPC Ribbon Album)

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
