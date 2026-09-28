# Lazeeza launcher

Home-screen icon for the Lazeeza app (a Google Apps Script web app, whose page Google
owns, so iOS can't take our icon from it). Added to the iPhone Home Screen from the
app's "Home Screen icon" button, this page shows the Lazeeza logo and forwards
straight into the app.

The app's private key is never in this repo or on this site: it travels after `#`
in the bookmarked link, which browsers never send to a server.

Android: `manifest.webmanifest` makes it an installable app (the `?setup` page has an Install
button). The installed app opens without `#k=`, so the key from the link is kept in this site's
storage on the phone. The manifest is added only on Android and other non-Apple phones: iOS would
open the manifest's start page without the key.
