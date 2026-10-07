# PixelFactoryResources

Public home of the four player-facing web pages for **Pixel Depot**
(the app whose code lives in the private repo `wanggit/PixelFactory`).
Served by GitHub Pages from this repo's `main` branch, root directory.

| Page | URL |
|---|---|
| Marketing / home | https://wanggit.github.io/PixelFactoryResources/ |
| Privacy Policy | https://wanggit.github.io/PixelFactoryResources/privacy/ |
| Terms of Use | https://wanggit.github.io/PixelFactoryResources/terms/ |
| Support | https://wanggit.github.io/PixelFactoryResources/support/ |

These are the URLs filed in App Store Connect (Marketing / Privacy / Support)
and opened from the app's Settings screen (`AppLinks` in
`lib/meta/links.dart`). Change them there and in `docs/urls.md` together.

## Editing discipline

The pages are **rendered from the private repo's copy sources**, not written
here first:

- `docs/product.md` + `docs/features.md` + `docs/marketing.md` → `index.html`
- `docs/privacy.md` → `privacy/index.html`
- `docs/terms.md` → `terms/index.html`
- `docs/support.md` → `support/index.html`

Edit the `.md` source in `wanggit/PixelFactory`, then re-render the page here.
Player-facing copy must only describe mechanics that are actually in the build.
Internal notes live in HTML-comment-free `.md` sources; never put internal
notes in these HTML files (they are public).

`img/` holds the app icon, an og:image banner and single-artwork crops taken
from the level artwork contact sheet. The artwork crops are fixed-size
decoration; anything stretchable belongs in CSS.

Level hot-update bundles are **not** here — they live in
`wanggit/PixelFactoryLevels` (see `docs/hot_update.md`).
