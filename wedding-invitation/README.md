# Wedding invitation (English + Tamil)

Single static page: `index.html`. No build step.

## Edit
Open `index.html`. Set your WhatsApp number in `CONFIG.whatsapp` (digits only, with country code, e.g. 919876543210). All wording is in the `T` object (en / ta).

## Push to GitHub
git init
git add .
git commit -m "Wedding invitation"
git branch -M main
git remote add origin https://github.com/<your-user>/<repo>.git
git push -u origin main

## Deploy on Render (free Static Site)
1. Render dashboard > New > Static Site > connect the repo.
2. Build command: leave empty. Publish directory: `.`
(Or use New > Blueprint, which reads `render.yaml`.)
