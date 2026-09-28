# HeartDistance web (GitHub Pages user site)

Published as the repo `Marco-P-Keller/Marco-P-Keller.github.io` → https://marco-p-keller.github.io

- `/.well-known/apple-app-site-association` — universal links: `/join/*` opens the app
  (`applinks:marco-p-keller.github.io` in both app entitlements).
- `/join/?n=<name>&c=<code>` — the pairing invite every "Share the code" sends.
  With the app installed iOS opens it directly (`AppModel.handleDeepLink`);
  otherwise the page shows the code, copies it, and leads to the App Store.
- `/` — redirects to the App Store.

`.nojekyll` must stay, or GitHub Pages drops the `.well-known` folder.
To update: copy this folder's contents into that repo and push.
