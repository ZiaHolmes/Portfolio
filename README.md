# Zia Holmes — Portfolio

A four-page portfolio site: plain HTML + one shared CSS file. No build tools needed.

## Folder structure

```
zia-portfolio/
├── index.html      ← Home (open this first)
├── work.html       ← Selected work
├── about.html      ← About
├── contact.html    ← Contact
├── css/
│   └── styles.css  ← ALL styling for every page
├── images/         ← put your photos + project images here
└── files/          ← put resume.pdf here
```

## Open it in VS Code

1. In VS Code: **File → Open Folder…** and pick `zia-portfolio`.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click `index.html` → **Open with Live Server**. The site opens in your browser and refreshes every time you save.

## Editing tips

- **Text:** search for `[` to find every placeholder still left to fill in.
- **Colors & fonts:** change them once at the top of `css/styles.css` (the `:root` block).
  For example, `--green: #2F5A3B;` controls every green button and band.
- **Adding an image:** drop it in `images/`, then replace a placeholder box, e.g.

  ```html
  <!-- before -->
  <div class="placeholder h-360">[PROJECT 1 — cover]</div>
  <!-- after -->
  <img class="media h-360" src="images/project-1.jpg" alt="Short description of the image">
  ```

- **Logo:** replace `<div class="brand-mark">[MARK]</div>` with
  `<img class="brand-mark" src="images/logo.png" alt="">` on each page.
- **Résumé:** save it as `files/resume.pdf` and the buttons will link to it.
- **Contact form:** it doesn’t send yet. Create a free form at formspree.io and paste
  your form URL into the `action="…"` on the `<form>` in `contact.html`.

## Putting it online (free)

GitHub Pages, Netlify (drag-and-drop the folder) or Vercel will host this as-is.
