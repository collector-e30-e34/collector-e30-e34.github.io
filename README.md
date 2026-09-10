# ZWEI · GARAGE — an E30 & E34 enthusiast site

A static site (no build step, no dependencies) presenting a BMW E30 (Alpinweiss)
and a BMW E34 (Sterlingsilber): blueprint schematics, engines, gearboxes,
chassis, wheels, and photo galleries.

## Structure

```
index.html        landing page (the diptych)
e30.html          E30 technical file
e34.html          E34 technical file
photos/e30/       your E30 photos → name them 01.jpg … 06.jpg
photos/e34/       your E34 photos → name them 01.jpg … 06.jpg
```

Everything (CSS, JS, SVG schematics) is embedded in the HTML files, so the
site works by just opening `index.html` in a browser — no server needed.

## Adding your photos

Drop JPEGs into `photos/e30/` and `photos/e34/` named `01.jpg` through
`06.jpg`. Empty slots show a dashed placeholder until you fill them.
Recommended: landscape orientation, ~1600 px wide, exported at quality 80
(keeps the repo light and the page fast). Want more than six? Copy a
`<figure>` line in the Galerie section of the page and increment the number.

## Deploying free on GitHub Pages

1. Create a repository named `YOURUSERNAME.github.io` (public).
2. Push these files to the repository root:
   ```
   git init
   git add .
   git commit -m "ZWEI garage site"
   git branch -M main
   git remote add origin https://github.com/YOURUSERNAME/YOURUSERNAME.github.io.git
   git push -u origin main
   ```
3. Done — the site is live at `https://YOURUSERNAME.github.io` within a
   minute or two. (If you use a differently-named repo, enable Pages in
   Settings → Pages → Deploy from branch, and the URL becomes
   `https://YOURUSERNAME.github.io/REPONAME/`.)

### Custom domain (optional)

GitHub Pages supports custom domains for free (Settings → Pages → Custom
domain, plus a CNAME record at your registrar). The `.github.io` address
itself costs nothing and works fine for sharing.

## Renaming the site

"ZWEI·GARAGE" appears in the header/footer of each page and in the `<title>`
tags — search and replace to make it your own.

## Notes

- Private enthusiast site; not affiliated with BMW AG. No logos or badges
  are used, only text and original line drawings.
- Spec tables list the common European variants; figures are approximate
  factory values and vary by market and model year.

