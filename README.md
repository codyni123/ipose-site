# ipose-site

Marketing, support and privacy site for the ipose iOS app (App Store Connect app 6818018078,
source in the private `codyni123/ipose` repo). Plain HTML and CSS, no build step, no analytics,
hosted on GitHub Pages from `main`.

- Home: https://codyni123.github.io/ipose-site/ (App Store "Marketing URL")
- Support: https://codyni123.github.io/ipose-site/support/ (App Store "Support URL")
- Privacy: https://codyni123.github.io/ipose-site/privacy/ (App Store "Privacy Policy URL", and the
  app's Profile and paywall links)

## Editing

Edit, commit, push `main`; Pages redeploys in about a minute. Paths are relative so the site works
under `/ipose-site/` and locally (`python3 -m http.server` from this folder); only `404.html`
uses absolute `/ipose-site/` paths.

- Colours follow the app: Paper in light mode, Graphite in dark (`style.css` tokens), the system
  font, monochrome, green only for "ready".
- `img/shots/*.jpg` are 600 px captures of the app (the App Store raw captures in the app repo's
  `marketing/screenshots/raw/`, resized).
- `img/appstore-badge.svg` is Apple's official badge artwork: don't restyle it. Until the app is
  live, the line under it says "Coming soon"; remove it at launch.
- The support email is a `mailto:` link, never visible text.
- Keep the privacy policy in step with the app's App Privacy answers (Data Not Collected) and
  `App/Resources/PrivacyInfo.xcprivacy`. If the app ever collects anything, this page changes first.
- `google4733d915db45d4de.html` and the `google-site-verification` meta tag are Search Console
  ownership proofs; don't delete them.
