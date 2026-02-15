# Config Your App

In order to configure this app to your session each convention and/or year, the following steps should be taken

- [ ] Update `app_config.json` 
  - [ ] Convention Name (with Year)
  - [ ] App Name
  - [ ] App URL (link to the website)
  - [ ] Discussion Board Link (i.e. Discord)
  - [ ] Ribbon Update Form (for users to submit ribbons)

- [ ] Update `Ribbons.csv` List of Ribbons at Convention
- [ ] Background Image
- [ ] Update QR Code Image

## Update `Config/Ribbons.csv`

Recommended columns (example):

- `file_name` (required): image filename (e.g., `dealer-app.png`)
- `name`
- `dealer`
- `type`
- `how-to-earn`
- `dealer-cosplay`
- `fandom`
- `days`

### Rules

- `file_name` must exactly match the image file in `Config/ImageRibbons/`
- Filenames are case-sensitive (`.png` is not `.PNG`)

### Update images

1. Add/replace images in `Config/ImageRibbons/`
2. Make sure the CSV `file_name` matches

## `BackgroundImage.png` (NPC background image)

- Purpose
  -This is the main visual of the page.
  - Should feel like an NPC scene (game-like).
- Guidelines
  - Recommended aspect: works best as a portrait-friendly image for phones.
  - Keep the NPC visually centered or slightly above center (dialog is at bottom).
  - Avoid tiny details near the bottom edge (they’ll be covered by the dialog box).

## `ImageQR.png` Link for users

Use a website like [qrcodemonkey](https://www.qrcode-monkey.com/) to generate a new URL based on your git pages, or where your website will be hosted at.

## `Conversations.json` (NPC dialog + menus)

### Purpose

- Controls the NPC-style dialog text and the choices users can pick.
- Keeps the app easy to expand without rewriting code.

### Key concepts

- Each node has an ID (like "start", "ribbons", "about").
- Each node can have:
  - text (what the NPC says)
  - choices (buttons)
  -optional view (special screens rendered from the CSV, like dealer/fandom lists)

### Choice fields

- label: (required) button text
- next: go to another conversation node
- url: open an external link in a new tab
- action: perform an app action 
  - back - will go back to the previous conversation
  - share - will use phone's "share" to text link
  - detail_dealer - will show a list of dealers, and their ribbons
  - detail_fandom - will show a list of fandoms, and their ribbons
  - open_ribbon_form - send link from `app_config.json` for traders to update their ribbons
  - open_discussion - send link from `app_config.json` for users to join a discussion board
  