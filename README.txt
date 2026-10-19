GAMBIA RCT PUPIL SAMPLER - INSTALLABLE VERSION (algorithm GMB-PS3.0)

WHAT IS IN THIS FOLDER
index.html            the app
sw.js                 makes it work with no signal after the first visit
manifest.webmanifest  lets phones install it to the home screen
icon-*.png            app icons
Upload ALL files to the same folder on a web host. Do not rename them.

HOSTING (needs https)
Any static host works: GitHub Pages, Netlify, Cloudflare Pages, or a MoBSE or
Think Equal web server. Nothing is sent to the host; names stay on each phone.
Offline install only works over https (or localhost), not from a file or http.

ENUMERATOR STEPS (once, with signal)
Android: open the link in Chrome. Tap "Install app" on the home screen of the
         tool, or Chrome menu > Install app / Add to Home screen.
iPhone:  open the link in Safari. Tap Share > Add to Home Screen.
Then open the app once from the home screen while online. After that it works
with no signal.

IMPORTANT
- Data stays on the phone, tied to this web address. If the address changes,
  the new address shows an empty list. Choose the address first and keep it.
- Save the names file for MoBSE after every school.
- To release a changed version, edit CACHE in sw.js and upload all files. Do not
  change the app once baseline sampling has started: it would break
  reproducibility.
