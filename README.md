# Remindfulness website (static, GitHub Pages)

The complete replacement for remindfulnessapp.com: six pages, one stylesheet, no build step.

## Files
- index.html — home
- classic.html, recovery.html, twin-flame.html — edition pages
- faq.html — FAQ + support (email link, no form)
- privacy.html — updated privacy policy (mentions AdMob, ATT, on-device reminders)
- css/style.css — all styling
- assets/ — DROP YOUR IMAGES HERE (see below)

## Images to add to /assets (exact filenames)
- classic-hero.png — panel 1 of the Classic App Store set (teal)
- recovery-hero.png — panel 1 of the Recovery set (purple)
- twinflame-hero.png — panel 1 of the Twin Flame set (peach)
- book.png — the book cover mockup
Until an image exists, its slot hides itself automatically, so the site works from day one.

## Two TODOs in the code
1. Twin Flame App Store links: search for "idTF" in index.html and twin-flame.html and replace with TF's real Apple ID (e.g. id1234567890) once the app is live.
2. GetResponse: in index.html, find the comment "Paste your GetResponse form embed code" and paste your embed there.

## Putting it live (preview first — Weebly stays untouched)
1. On GitHub, create a new repository named remindfulnessapp-site (public).
2. Upload everything in this folder (drag and drop onto the repo page, "Add file > Upload files").
3. Repo Settings > Pages > Source: Deploy from a branch, Branch: main, folder: / (root). Save.
4. After a minute the site is live at: https://njanzenapps.github.io/remindfulnessapp-site/
5. Review it on your phone and computer. Weebly keeps serving remindfulnessapp.com meanwhile.

## Switching the real domain over (only when happy)
1. In the repo: Settings > Pages > Custom domain: www.remindfulnessapp.com > Save (this creates a CNAME file).
2. At your DNS host for remindfulnessapp.com: point the www CNAME to njanzenapps.github.io, and the root @ A records to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153.
3. Back in GitHub Pages settings, tick Enforce HTTPS once the check passes.
4. Weebly can then be cancelled, but export/save anything you want from it first (blog posts, old images).

## Notes
- The support email shown is support@remindfulnessapp.com — make sure that address exists/forwards, or change it in faq.html and privacy.html.
- The App Store badge is loaded from Apple's official asset URL; if you'd rather self-host it, download the SVG into /assets and update the src.
- Fonts load from Google Fonts (Abril Fatface + Jost).
