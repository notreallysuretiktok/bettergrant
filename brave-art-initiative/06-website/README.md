# Website

## Step 1: Which GoDaddy product is it?

Log in to GoDaddy, open **My Products**, and see which of these the site is under. It changes how we build.

| GoDaddy product | How we'd build it |
|---|---|
| **Websites + Marketing** (drag-and-drop builder) | You can't upload custom code. We write the copy, prep web-sized images, and lay out each section so you can rebuild it in the editor. |
| **Web Hosting (cPanel)** | Full custom site built in this repo. You upload it through cPanel File Manager, or we set it to deploy automatically from GitHub. |
| **Managed WordPress** | Pick a theme, then we write the pages and you paste them in, or we build a custom theme. |

## Sitemap (draft)

```
Home
About
  ├─ Our Story (founder)
  └─ Mission
Programs
Projects
  ├─ Peeling Back the Prophecy
  ├─ God & Country
  ├─ Kitty Kat Whisker
  └─ Life After the Cult
Media (podcasts, press, media kit download)
Get Involved
  ├─ Donate
  └─ Volunteer / Partner
Contact
```

## Home page, top to bottom

1. **Hero**: big line "Heal loudly." Under it: "Brave Art Initiative helps veterans and survivors turn pain into purpose through art, storytelling, and real conversation." Two buttons: **Donate** and **Our Story**.
2. **The problem**: a short paragraph and one statistic about veterans coming home.
3. **What we do**: 3 cards, one per program.
4. **Founder quote**: "I didn't find peace when I came home. I had to build it." with Drew's photo and a link to Our Story.
5. **Projects strip**: the book and series covers in a row.
6. **As heard on**: podcast logos.
7. **Get involved**: Donate / Volunteer / Partner.
8. **Footer**: newsletter signup, Instagram, contact, EIN and nonprofit status line.

## Web image specs

| Use | Size | Format | Target file size |
|---|---|---|---|
| Hero background | 2400 px wide | WebP + JPG fallback | under 400 KB |
| Project covers | 1024 × 1536 | WebP | under 250 KB |
| Headshots | 1200 px tall | WebP / JPG | under 250 KB |
| Logo | — | SVG + PNG | — |
| Favicon | 512 × 512 | PNG + ICO | — |
| Social share image | 1200 × 630 | JPG | under 300 KB |
