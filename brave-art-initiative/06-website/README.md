# Website

**Domain:** [braveartinitiative.com](https://braveartinitiative.com): registered at GoDaddy, served free from GitHub Pages

**Worth grabbing:** `braveartinitiative.org` was still unregistered as of 2026-10-21. Most donors expect a nonprofit to be on .org, so register it and forward it to the .com before someone else takes it.

## The site

Version 1 is in `site/`: a single page with no build step. To preview it, open `site/index.html` in a browser.

```
site/
  index.html     ← all page content
  styles.css     ← colors, fonts, layout
  favicon.svg
  fonts/         ← Bebas Neue, Cormorant Garamond, Inter (self-hosted, SIL Open Font License)
  images/        ← covers + og-image.jpg (the preview image when the link is shared)
```

**Contact:** braveartinitiative@gmail.com. **Donate:** Cash App [$streetsoldiersmn](https://cash.app/$streetsoldiersmn), linked from the header and the Connect section.

**Still to add:** a photo of Drew.

## Going live (GitHub Pages)

Any change to `site/` that lands on `main` is published automatically by `.github/workflows/deploy-website.yml`.

### One-time setup

**1. Turn on Pages in GitHub**
Repo → **Settings** → **Pages** → under *Build and deployment*, set **Source** to **GitHub Actions**.

**2. Get the site onto `main`**
Merge the pull request. The site goes live at `https://notreallysuretiktok.github.io/bettergrant/` within a couple of minutes (check the **Actions** tab).
If the first run fails because Pages wasn't on yet, open **Actions** → **Deploy website** → **Run workflow**.

**3. Point the domain at GitHub (in GoDaddy)**
GoDaddy → **My Products** → braveartinitiative.com → **DNS** → *DNS Records*:

| Type | Name | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | notreallysuretiktok.github.io |

- Edit the existing `@` A record (it may say *Parked*) to the first IP, then add the other three.
- Delete any other `@` A records, and turn off **Forwarding** for the domain if it's on.
- If GoDaddy says a record is managed by *Websites + Marketing*, disconnect the domain from that site first.

**4. Connect the domain in GitHub**
Repo → **Settings** → **Pages** → **Custom domain**: `braveartinitiative.com` → **Save**.
Once the DNS check passes, tick **Enforce HTTPS**. DNS can take from minutes to a few hours, and the HTTPS certificate up to about an hour after that.

**Recommended:** verify the domain under your GitHub account's **Settings** → **Pages** so nobody else can ever attach it to their own GitHub site.

### Updating the site later

Edit files in `site/`, then merge to `main`. It republishes on its own.

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
