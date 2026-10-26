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
- To release a changed version, upload all the new files and change the CACHE
  name in sw.js (for example -r2 to -r3). Wait about 10 minutes. Phones update
  after being closed and reopened once or twice with signal. The Build number at
  the bottom of the app shows which version a phone has. Saved schools are kept.
- Do not change the sampling engine once baseline has started: saved schools
  would show a "no longer reproduces" warning.

BUILD HISTORY
r1  first release
r2  added school EMIS code and learner gender (Female/Male); build number shown
r3  shorter Child IDs (e.g. 0123-01-19); warns if a school code is sampled twice on a phone
r4  EMIS code is now the only school code; up to 9 ECD classes; Completed / Edit lock for each school; Status columns in exports
