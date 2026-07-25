# Mittalji Laddoo Wale — Coming Soon

A single-page "coming soon" site for **Mittalji Laddoo Wale**, an Indian sweets (mithai) brand serving both national (India) and international customers.

## Preview

Open `index.html` directly in any browser — no build step, no dependencies to install.

## Structure

```
.
├── index.html          # the whole page: markup, styles, and script in one file
├── assets/
│   └── mittalji-logo.png   # brand logo, transparent background
└── README.md
```

## Notes

- Pure HTML/CSS/JS. No framework, no bundler.
- Fonts (`Rozha One`, `Karla`, `Noto Sans Devanagari`) load from Google Fonts via `@import` in the `<style>` block — an internet connection is needed for them to render; the page still works without it, just falls back to system fonts.
- The "Notify Me" form is front-end only right now (`index.html`, bottom `<script>` block) — it shows a confirmation message but doesn't send anywhere. Wire the `fetch()`/form action up to your email provider (Mailchimp, Formspree, a custom API, etc.) before going live.
- Respects `prefers-reduced-motion`.

## Deploying

Works as-is on any static host — GitHub Pages, Netlify, Vercel, S3, etc. For GitHub Pages:

1. Push this repo to GitHub.
2. Repo **Settings → Pages** → set source to the `main` branch, root folder.
3. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## License

Add a license of your choice (e.g. MIT) if you plan to make this repo public.
