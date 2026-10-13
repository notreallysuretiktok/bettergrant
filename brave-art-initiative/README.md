# Brave Art Initiative — File System

One home for everything Brave Art Initiative (BAI): brand, creative projects, programs, press, grants, and the website.

> **This repo is public.** Only put things here that you'd be fine with anyone reading.
> These stay **out** of this repo (keep them in a private Google Drive or a private repo):
> 501(c)(3) letter, EIN, bylaws, bank/donor info, contracts, anything under NDA (the docu-series),
> and photos of minors unless you've cleared them.

## Map

| Folder | What lives here |
|---|---|
| `01-brand/` | Logos, colors, fonts, social/flyer templates, brand guide |
| `02-projects/` | One folder per creative project (books, series, covers) |
| `03-programs/` | What BAI actually runs: workshops, classes, events, who they serve |
| `04-media-kit/` | Founder bio, headshots, talking points, podcast/press appearances |
| `05-grants/` | Reusable grant boilerplate, budgets, applications, awards |
| `06-website/` | Sitemap, page copy, web-ready images, and the site build |

## Naming convention

```
bai_<area>_<thing>_<variant>_v<NN>.<ext>
```

- All lowercase, hyphens inside words, underscores between parts
- Dates as `YYYY-MM-DD` so they sort correctly
- Bump the version instead of writing `final`, `final2`, `FINAL-really`

Examples:

```
bai_logo_primary_full-color_v01.svg
bai_logo_icon_white_v01.png
bai_prophecy_cover_front_v03.jpg
bai_media_podcast-one-sheet_2026-10-13.pdf
```

## New project?

Copy `02-projects/_template/` to `02-projects/<project-name>/` and fill in its README.
