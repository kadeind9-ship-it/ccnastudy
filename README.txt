CCNA LAB NOTEBOOK — MOBILE APP (PWA)
=====================================

WHAT'S IN THIS FOLDER
  index.html    the entire app
  manifest.json app name, icon, fullscreen settings
  sw.js         service worker (makes it work offline)
  icon-192.png  home screen icon
  icon-512.png  splash/install icon
  README.txt    this file

GET IT ON YOUR PHONE (about 3 minutes, free)

STEP 1 — Host the folder (pick one):
  Option A: Netlify Drop (easiest)
    1. Go to https://app.netlify.com/drop
    2. Drag this entire folder onto the page
    3. It gives you a URL like https://something.netlify.app
  Option B: GitHub Pages
    1. Create a repo, upload these 5 files
    2. Settings -> Pages -> deploy from main branch
    3. URL: https://yourname.github.io/reponame

STEP 2 — Install on your phone:
  iPhone (Safari):
    1. Open your URL in Safari
    2. Tap the Share button
    3. Tap "Add to Home Screen"
  Android (Chrome):
    1. Open your URL in Chrome
    2. Tap the three-dot menu
    3. Tap "Add to Home screen" / "Install app"

THAT'S IT
  - Launches fullscreen with its own icon, no browser bars
  - Works offline after the first visit (service worker caches it)
  - Progress saves on your device (localStorage) and survives
    closing the app, restarting your phone, etc.
  - To update the app later: replace index.html on your host

NOTE
  Opening index.html directly in a phone browser (without hosting)
  also works for studying, but "Add to Home Screen" install and
  offline mode require it to be served over https — hence step 1.
