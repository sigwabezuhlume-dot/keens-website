# Keen's World — Website

A one-page site for Keen: hero banner, about section, picture gallery, and
contact links (WhatsApp + email).

## Files

```
keens-world/
├── index.html      → the page content
├── style.css        → all styling (colors, fonts, layout, background)
├── README.md         → this file
└── images/
    ├── keen_logo_background_subtle.png   → full-page background
    └── images.jpeg                        → photo used in the gallery
```

All three files (`index.html`, `style.css`, and the `images` folder) need to
stay together in the same folder, in this same relative arrangement, or the
page will lose its styling and images.

## How to view it

Double-click `index.html` — it opens directly in any web browser (Chrome,
Safari, Edge, etc.). No install or server needed.

## How to put it online

Any basic web host works. A few free/easy options:

- **Netlify / Vercel**: drag the whole `keens-world` folder onto their
  upload page and it goes live in seconds.
- **GitHub Pages**: create a repo, upload these files, turn on Pages in the
  repo settings.
- **Existing hosting (e.g. from a domain provider)**: upload the contents of
  this folder to the `public_html` (or similar) folder via their file
  manager or FTP.

## Making common edits

Open `index.html` in any text editor (Notepad, TextEdit, VS Code, etc.).

- **Change the music link**: search for `ditto.fm/new-horizons-keen` — it
  appears in the nav, the hero button, and the About text. Replace it with
  a new link everywhere it appears.
- **Change the WhatsApp number**: find `https://wa.me/27619970825` and
  replace the digits with the new number in international format (country
  code, no `+`, no spaces, no leading `0`).
- **Change the email address**: find `mailto:szuhlume@gmail.com` and swap
  in the new address (in both places it appears — the `href` and the
  visible text).
- **Add more gallery photos**: put new image files in the `images` folder,
  then in `index.html` copy a line like:
  ```html
  <div class="gallery-item">
    <img src="images/your-new-photo.jpg" alt="Describe the photo" />
  </div>
  ```
  and paste it inside the `<div class="gallery">` block, replacing a
  `placeholder` item.
- **Change colors/fonts**: open `style.css` and edit the values at the very
  top under `:root` — `--gold`, `--ink`, `--mist`, `--white` control the
  color scheme site-wide.

## Notes

- The background image is fixed and set to fill the entire screen
  (`background-size: cover`) on every device size.
- The site is responsive — it reflows for phones and tablets automatically.
