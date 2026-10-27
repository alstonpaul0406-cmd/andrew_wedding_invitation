# Andrew & Carmel — Catholic Wedding Invitation

Static Render-ready wedding invitation.

## Folder
- `index.html` — complete invitation
- `render.yaml` — Render Static Site configuration
- `assets/catholic-wedding.png` — animated-style Catholic wedding illustration used in the invitation

## Deploy on Render
1. Upload this folder to a GitHub repository.
2. In Render, choose **New → Static Site**.
3. Select the repository and deploy the `main` branch.
4. Build command: leave empty.
5. Publish directory: `.`

The site is plain HTML/CSS/JavaScript and needs no build step.

## Customize
Open `index.html` and edit the `CONFIG` object near the bottom:
- `start` — wedding date/time
- `whatsapp` — RSVP WhatsApp number, digits only
- `maxGuests` — maximum RSVP guest count
- `start3` / `durationHours3` — third event
- `music` — optional path such as `music/song.mp3`
- `musicVolume` — 0 to 1

The English and Tamil wording is in the `T` object.

The main Catholic wedding illustration is:
`assets/catholic-wedding.png`

The illustration is given a gentle CSS float/zoom animation so it feels alive without requiring a video file.
