# motoshige496.github.io

Personal homepage of **Motoshige Sato (佐藤元重)** — Postdoctoral Scholar, Chang Lab, UCSF.

Live site: <https://motoshige496.github.io/>

## Structure

A single static page, no build step and no dependencies.

| File | Purpose |
|---|---|
| `index.html` | The whole site — markup, CSS and JS inline |
| `face.jpg` | Portrait used in the hero section |
| `google2dbc9b369b260355.html` | Google Search Console verification for the old domain |

`mystyle.css`, `title.gif` and `default_page.png` are leftovers from the pre-2026
version of the site and are no longer referenced.

## Editing

Open `index.html` and edit it directly. Pushing to `main` publishes the site
via GitHub Pages.

### Bilingual content

The page is bilingual, English by default. Each translated fragment is a pair of
elements marked with `data-l`:

```html
<span data-l="en">Postdoctoral Scholar</span><span data-l="ja">博士研究員</span>
```

CSS hides whichever language is not active, based on `data-lang` on `<html>`.
The toggle in the header sets it and remembers the choice in `localStorage`;
`?lang=ja` forces Japanese on first visit.

**When adding a publication or an entry, add both languages.** If a line is
identical in both (most English-language citations), no pair is needed.

## Previous hosting

The site used to live at `motoshigesato.encoder.jp` on StarServer. That address
now 301-redirects here — see `_starserver_redirect/` in the working copy
(not committed) for the files that implement it.
