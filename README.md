# SiteHired — website

The public website for **SiteHired**, an AI-powered marketplace that matches UK construction companies with fully-vetted workers.

**Live:** [sitehired.com](https://sitehired.com)

## What's here

A fast, dependency-free static site, built from the SiteHired brand system ("Engineered Calm") and approved copy.

| Page | File |
|---|---|
| Homepage | `index.html` |
| For companies | `for-companies.html` |
| For workers | `for-workers.html` |
| Contact (with form) | `contact.html` → `thanks.html` |
| Privacy | `privacy.html` |
| Not found | `404.html` |

```
assets/
  styles.css      all styles + brand colour tokens
  fonts/          Instrument Sans + Geist Mono (self-hosted, SIL OFL)
  img/            favicon, touch icon, social share image
```

## Design decisions

- **No framework, no build step.** Plain HTML and one stylesheet, so it's easy to hand over, loads quickly, and hosts anywhere.
- **Swappable palette.** Colours are CSS custom properties (`--sh-ink`, `--sh-accent`, …). The three candidate brand palettes are in the top of `assets/styles.css`; switching is a one-block change.
- **Accessible contrast.** Accent colours have darker and lighter text variants so small text passes WCAG AA on light and dark backgrounds.
- **Privacy-friendly.** Fonts and images are self-hosted, with no cookies, analytics or third-party requests.
- **Responsive.** Tested at desktop and phone widths, with no horizontal scroll.

## Hosting

Deployed on [Netlify](https://www.netlify.com). The contact form uses Netlify Forms (`data-netlify="true"` plus a honeypot field). Any static host works for the rest of the site.

## Credits

Brand system and copy: SiteHired team. Built by George McCrae.
