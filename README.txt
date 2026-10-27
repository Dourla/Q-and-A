BIBLE ANSWERS — installable app
===============================

What is in this folder
  index.html            the whole app (662 Telugu questions, 39 themes, 8 groups)
  manifest.webmanifest  makes it installable (name, colours, icons)
  sw.js                 service worker — offline support
  icons/                home-screen icons (192, 512, maskable, apple-touch, favicon)

How to put it online (2 minutes, free)
  Option A — Netlify Drop
    1. Go to https://app.netlify.com/drop
    2. Drag this whole "bible-answers" folder onto the page.
    3. You get a web address. Open it on your phone.

  Option B — GitHub Pages
    1. Create a repository and upload these files (keep the icons folder).
    2. Settings → Pages → Branch: main → Save.
    3. Open the published address.

  Option C — test locally
    In this folder run:  python3 -m http.server 8080
    Then open http://localhost:8080

Install on the home screen
  Android / Chrome: open the address → menu (⋮) → "Install app" (or the install
    icon in the address bar). The Q&A Bible icon is added to your home screen.
  iPhone / iPad: open the address in Safari → Share → "Add to Home Screen".
  Windows / Mac (Chrome, Edge): install icon in the address bar → Install.

Notes
  • After the first visit the app works offline — questions, answers, notes,
    saved list and studied marks are all stored on the device.
  • Looking up a Bible verse needs internet the first time; verses you have
    opened are then cached for offline use.
  • Settings → Backup saves your notes and marks to a file; Restore brings
    them back on another device.

  If you only have the single HTML file (Bible_Answers_Pro.html), it works the
  same way when opened in a browser, but installing from a file:// path is
  limited — host this folder to get a real installable app.
