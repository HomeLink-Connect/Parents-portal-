WISE PARROT PARENT PORTAL — installable app
============================================
Upload ALL of these together to the same HTTPS folder (Firebase Hosting, Netlify, GitHub Pages, cPanel with SSL):

  index.html              the portal (all logic + embedded logo)
  manifest.webmanifest    app name, colours, icons, shortcuts
  sw.js                   service worker (offline + fast loading)
  icons/                  app icons (Wise Parrot crest)

Installing is only offered over HTTPS (or localhost). Opening index.html directly from a
phone's files will still work as a normal page, but it can't be installed.

Android / Chrome : "Install the Wise Parrot app" button appears on the login screen.
iPhone / Safari  : the same button shows Share -> Add to Home Screen steps.

When you publish a new version, change VERSION in sw.js (e.g. wp-parent-v2) so phones refresh.
