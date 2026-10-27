# Wedding invitation (English + Tamil)

Single static page: `index.html`. No build step.

## Folder layout
```
index.html
render.yaml
images/   couple.jpg, photo1.jpg ... photo6.jpg
music/    song.mp3
```

## Edit
Open `index.html` and find the `CONFIG` block near the bottom:
- `whatsapp`: digits only, with country code, e.g. 919876543210
- `hero`: round photo at the top (optional)
- `photos`: gallery list. Add or remove file names freely; missing files are skipped, and the gallery hides if none load
- `music`: background music file (optional); `musicVolume` is 0 to 1

All wording is in the `T` object (en / ta).

## Photos
- JPG, about 1200 px on the long side, under 300 KB each (phones on mobile data will thank you).
- Name them exactly as in `CONFIG.photos`, or change the names there.

## Music
- MP3, ideally under 4 MB (trim to 2 to 3 minutes; it loops). Use a song you have the rights to use.
- Browsers block autoplay, so music starts when the guest taps "Open invitation". A round music button (bottom-left) lets them mute it.

## Push to GitHub
git init
git add .
git commit -m "Wedding invitation"
git branch -M main
git remote add origin https://github.com/<your-user>/<repo>.git
git push -u origin main

Later updates: `git add . && git commit -m "Update" && git push`. Render redeploys automatically.

## Deploy on Render (free Static Site)
1. Render dashboard > New > Static Site > connect the repo.
2. Build command: leave empty. Publish directory: `.`
(Or use New > Blueprint, which reads `render.yaml`.)
