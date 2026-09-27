# Inspirational Consultations

Static website for Jenny Biancotti's social work practice, Inspirational Consultations (Mount Lawley, Perth WA). Hosted on GitHub Pages.

## Repo structure

```
index.html          the entire site — one file, no build step
assets/             every image the page loads
favicon.ico         root copy, for browsers that ask for /favicon.ico
README.md           this file
```

Nothing else belongs at the root. `index.html` references images as `assets/…` only.

## Assets

All filenames are lowercase with no spaces. GitHub Pages is case-sensitive, so keep them exactly as named.

| File | Used for |
|---|---|
| `tree-icon.png` | logo in the sticky header |
| `tree-hero.png` | large tree beside the hero heading |
| `tree-watermark.png` | faint background behind Acknowledgement of Country |
| `logo-full.png` | footer logo |
| `jenny-photo.jpg` | portrait in "A bit about me" |
| `aasw-badge.png` | AASW membership badge under the portrait |
| `differing-perspectives-cover.jpg` | thumbnail in the Publications accordion |
| `seedling.jpg` | beside the Brené Brown quote in "Why Inspirational Consultations?" |
| `consulting-room.jpg` | Mount Lawley consulting room, in the Location section |
| `og-image.jpg` | social share preview |
| `favicon-16.png`, `favicon-32.png`, `favicon-180.png`, `favicon.ico` | browser and Apple touch icons |

`favicon-48.png`, `favicon-512.png` and `tree-transparent.png` are not referenced by `index.html`. Safe to delete unless a web app manifest gets added later.

## Before going live

1. In `index.html` `<head>`, replace `REPLACE-WITH-DOMAIN` with the real domain, or social share previews won't load.
2. Confirm the wording and source of the second Brené Brown quote in the "Why" section. It is currently attributed to Brené Brown with no book cited, unlike the "My Approach" quote which cites *The Gifts of Imperfection*. Add a source line if one can be verified.
3. The contact form has no backend. It shows a success message but does not send anything.

## Content decisions

- **Fees are not published.** The fee grid was removed in September 2026 at Jenny's request and replaced with "contact me to discuss fees and availability". Do not reinstate it.
- **Jenny's bio and the "Why" copy are her own words**, supplied verbatim. Don't edit for style without asking.

## Editing

There is no build step. Edit `index.html` directly, commit, and GitHub Pages republishes within a minute or two. All CSS and JavaScript live inside that one file.
