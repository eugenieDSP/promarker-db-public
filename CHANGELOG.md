# Changelog — Promarker Studio (public)

Version numbers match the service-worker cache version (`sw.js`), bumped on
every release so installed copies pick up the update.

The app currently includes **4 brands / 943 colours**: Promarker (205),
Copic (263), Ohuhu (319), Prismacolor Premier (156).

> Note on brand order: the app began as a **Promarker-only** tool. Additional
> brands were added over time in this order: **Ohuhu, then Prismacolor, then
> Copic.** (The exact release these each landed in is reconstructed from memory;
> the sequence is correct even where a version number is approximate.)

---

## v1 — Initial public release
- Standalone, offline PWA. Starts empty; users build their own collection.
- **Single brand at launch: Winsor & Newton Promarker.**
- Tabs: Collection, Colour wheel, About.
- Photo eyedropper: measure a swatch's real colour in 1, 2 and 3 ink layers.
- Per-layer readouts: hex, RGB, approximate Munsell notation, hue / chroma / saturation.
- Harmonies (complementary, analogous, triadic, split-complementary) from your collection.
- Munsell-style hue–chroma colour wheel.
- Local-only storage — no account, no server, no analytics. Export / import backup.
- Installable to home screen; works fully offline. In-app-browser warning banner.

## v2 — Reverse colour lookup
- New **Find** tab: paste a hex or RGB value, get the closest markers by
  CIELAB ΔE, with scope options.

## v3 — Storage hardening
- Saves now verify themselves (read back after writing).
- Deep-copied in-memory fallback so a failed save can't corrupt data.
- Persistent "storage blocked" warning when the browser disallows storage.
- Fixed a first-launch crash that could occur when storage was unavailable.

## v4 — Ohuhu brand added (first brand beyond Promarker)
- Added the **Ohuhu** range (319 colours; codes and names transcribed from the
  Honolulu chart, colours as flagged estimates).
- App becomes multi-brand: brand filter row, brand tags on cards, and
  cross-brand substitution introduced in Find.

## v5 — Bug fix
- Fixed a crash caused by an unescaped apostrophe in the About text.

## v6 — Prismacolor brand added
- Added the full **Prismacolor Premier** range (156 colours).

## v7 — Add-colours improvements
- Sticky **Close** button on the Add-colours popup (stays visible while scrolling).
- **Colour-group (family) filter** alongside the brand filter in the range picker.
- Fixed a stale "From the Promarker range" label (now "From the ranges").

## v8 — Cross-brand equivalents
- Every colour's detail view now lists its closest match in each other brand,
  with the ΔE distance.

## v9 — Browse tab, fuller harmonies, better Find defaults
- New **Browse all** tab: the whole catalogue across every brand, with brand +
  colour-group filters, search, and an owned-count.
- Harmonies now search the **full range**, not just your collection (owned shown
  solid, unowned dashed).
- Find now defaults to all-brands, so results include owned and unowned markers.

## v10 — Universal detail popups
- Every colour opens a detail view, whether or not you own it.
- Unowned colours open read-only with an **Add to collection** button.
- Harmony chips and cross-brand substitute rows are all tappable.

## v11 — Copic brand added + Wishlist
- Added the **Copic** range (263 colours), completing the current four-brand
  catalogue (943 colours total).
- **Wishlist:** wishlist any unowned colour (♡ toggle in its detail view).
  Wishlist section on the Collection tab; ♡ badges in Browse; count in the header.
  Adding a colour to your collection clears its wishlist flag. Included in
  export / import backups; cleared by "Erase everything".

---

*Not affiliated with or endorsed by Winsor & Newton, Copic, Ohuhu, Prismacolor,
or any marker maker. Brand and colour names are used only to identify products.*
