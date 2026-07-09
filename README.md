# Promarker Studio

## New here? Start with this

**Promarkers** are alcohol-based twin-tip marker pens made by Winsor & Newton, popular for illustration, sketching, and colouring. They come in a big range of colours, each with a short code printed on the pen (like `Y657` or `B346`). Once you own more than a handful, two problems show up: it's hard to remember which ones you have, and the tiny colour dots on shop charts rarely match what the ink actually looks like on paper.

**This app fixes both.** It's a free tool where you list the markers you own, capture what they *really* look like from a photo of your own swatches, and find colours that go nicely together. It runs in your web browser, keeps everything on your own device, and needs no account.

> This is a fan-made tool. It is not made by, affiliated with, or endorsed by Winsor & Newton, Copic, Ohuhu, Prismacolor, or any marker maker. Brand and colour names are used only to identify the pens. Colour names and codes are used only to identify the pens.

## Opening this from a link (please read)

If you tapped a link from **Reddit, Instagram, Facebook, or a similar app**, it may have opened inside that app's own mini-browser. That mini-browser can forget your collection when you close it, and often won't let you install the app.

**Do this once:** open the little menu (usually `⋯` or a share icon) and choose **"Open in Safari"** / **"Open in Chrome"** / **"Open in browser"**. From there everything below works properly, and your collection will be safe. If you want to keep the app, also follow "Putting it on your phone or computer" further down.

---

A free little app for anyone who uses alcohol markers. It helps you keep track of which markers you own — across brands — see what colours they *really* make (screen swatches often lie), pick colours that work well together, and find the closest match in another brand when you want to substitute. It currently includes **Winsor & Newton Promarker**, **Copic**, **Ohuhu** (Honolulu range), and **Prismacolor Premier**, with a custom option for any other brand.

Everything stays on your own device. No sign-up, no account, no ads, nothing sent anywhere. It even works with no internet once you've opened it once.

> This is a fan-made tool. It is not made by, affiliated with, or endorsed by Winsor & Newton, Copic, Ohuhu, Prismacolor, or any marker maker. Brand and colour names are used only to identify the pens.

---

## What can it do?

- **Keep a list of the markers you own** — add them from the full official Promarker range with a couple of taps.
- **See real colours, not guesses** — take a photo of a swatch you've coloured, tap it, and the app records the true colour. It even shows what one, two, and three layers of ink look like.
- **Show the colour codes** — for every marker you get the HEX and RGB values (handy for digital work), plus hue, chroma and saturation.
- **Find matching colours** — open any marker to see which of your other markers go well with it (complementary, analogous, and so on).
- **Reverse colour search** — got a HEX or RGB value from somewhere? The **Find** tab tells you the closest marker to reach for, in your collection or any brand.
- **Filter by brand & find substitutes** — view one brand at a time, or use Find to see which Copic best matches a Promarker (or vice versa) when you want to swap between them.
- **A colour wheel** — see your whole collection arranged by colour, like a painter's wheel.

---

## How to start (the very first time)

When you open the app it's **empty** — that's normal. You tell it which markers you have.

1. Tap the **+ Add colours** button at the top.
2. Choose **From the Promarker range**.
3. Scroll or search, and tap **Add** next to each marker you own. (Don't worry about getting them all at once — you can come back anytime.)
4. That's it. Your markers now show up on the **Collection** tab.

Owned a marker that isn't in the list (an old or discontinued one)? Use **+ Add colours → Custom** to add it by hand.

---

## Recording a swatch's real colour (optional but the best bit)

Screen colours are only estimates. To capture how a marker *actually* looks on paper:

1. On paper, colour a small patch with your marker. For the best result, colour part of it once, part twice, and part three times (one, two, three layers).
2. Take a photo in **daylight, away from direct sun** — lamps make everything look orange.
3. In the app, tap the marker, then tap **Sample** next to "1 layer".
4. Choose your photo and **tap the spot** on it that shows that number of layers.
5. Tap **Use this colour**. Repeat for two and three layers if you like.

A little dot appears on markers you've measured, so you can see your progress.

---

## Keeping your collection safe

Your collection lives only in this browser, on this device. If you clear your browsing data, or switch phones, it won't magically follow you. So:

- Open the **About** tab and tap **Export backup** now and then. This saves a small file.
- To move to another device (or restore after clearing data), open the app there and tap **Import backup**, then pick that file.

There's also an **Erase everything** button in About if you ever want a fresh start.

---

## Putting it on your phone or computer like a real app

Once it's open in your browser you can "install" it so it gets its own icon and works offline:

- **iPhone / iPad (Safari):** tap the Share button, then **Add to Home Screen**.
- **Android (Chrome or Firefox):** open the menu (⋮), then **Add to Home screen** / **Install app**.
- **Computer (Chrome or Edge):** look for a small install icon in the address bar, or open the menu and choose **Install this page as an app**.

After that it opens full-screen, has its own icon, and works even with no internet.

---

## A couple of honest notes

- The colours the app starts with are **estimates** — for Copic and especially Ohuhu they're only a rough starting point (Ohuhu even varies pen to pen), so treat them loosely. They get accurate when *you* measure your own swatches from photos. Your phone's camera and lighting affect the result, so daylight gives the truest colours.
- The colour wheel positions are **approximate** — good for seeing the shape of your collection, not for exact colour science.
- Your data is **per device**. Use Export/Import (above) to move or back it up.

---

## For the person hosting this app

This is a "PWA" — a website that behaves like an app. To put it online for free with **GitHub Pages**:

1. Create a free account at github.com.
2. Make a new **public** repository (any name, e.g. `promarker-studio`).
3. Upload **all** the files from this folder (`index.html`, `sw.js`, `manifest.webmanifest`, and the three `icon-*.png` files) into it.
4. In the repository, go to **Settings → Pages**, set the source to your main branch, root folder, and save.
5. After a minute or two your app is live at `https://<your-username>.github.io/<repository-name>/`.

To update it later: upload the changed files again and commit. Because the app caches itself for offline use, whoever installed it should fully close and reopen it a couple of times to pick up the new version. (Whenever the app's contents change, bump the version number in `sw.js` — the line `const CACHE = "...-v1"` becomes `-v2`, etc. — so installed copies refresh.)

Not affiliated with or endorsed by Winsor & Newton. Colour names and codes are used only to identify products.
