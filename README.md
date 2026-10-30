# Valerie Hetherington's portfolio

A plain static site: HTML, CSS and two SVG illustrations. No build step, no dependencies, no JavaScript.

```
index.html       the page
styles.css       all styling; colors and fonts are at the top (:root)
404.html         shown for pages that don't exist
favicon.svg      browser tab icon
assets/
  hero.svg       the ski girl in the arch at the top
  about.svg      the cocoa illustration in the About section
  og-image.png   1200x630 link preview image
resume.pdf       résumé with contact details removed
```

## See it locally

From this folder:

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Put it online (GitHub Pages, free)

1. On GitHub, create a **public** repository named exactly `skifast.github.io`.
2. Upload everything in this folder to the repository's main branch (drag the files into the web page, or use git).
3. In the repository, go to Settings → Pages. Set the source to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at https://skifast.github.io.

Other hosts work too. On Netlify or Vercel you can drag this folder in and it deploys as is.

A custom domain (for example valeriehetherington.com) can be pointed at GitHub Pages in the same Settings → Pages screen.

## Résumé

`resume.pdf` is a copy of the résumé with the phone number and email removed. To update it, redo that removal on the new version before replacing the file, because anything on this site is public.

## Changing things

- **Colors:** edit the `--accent` line at the top of `styles.css`. Everything pink follows it.
- **Projects:** each ticket is one `<li>` in `index.html`. Copy one to add a project.
- **Text:** all copy is in `index.html`.
