# Beyond the Gate — Henty 2026 Landing Page

Static site. Two pages: `index.html` (signup) and `thank-you.html` (download reveal).

## Before going live

1. **MailerLite embed** — open `index.html`, find the block marked
   `MAILERLITE EMBED — REPLACE THIS BLOCK` and paste your real MailerLite
   embedded-form code in its place (the form tagged "Henty 2026").
2. **Redirect** — in MailerLite's form settings, set the success redirect to
   your live `/thank-you` URL once the site is deployed.
3. **Fonts** — Jost + Instrument Sans load from Google Fonts via `style.css`.
   No action needed as long as the live site has normal internet access.

## Structure

```
index.html          → landing page
thank-you.html       → download reveal page
style.css            → shared styles (all design tokens from the brief)
assets/              → hero image + 3 partner logos
downloads/            → the 3 PDF lead magnets
```

## Deploying

Push this whole folder to a GitHub repo, then import that repo in Vercel.
No build step / framework needed — deploy as a static site.
