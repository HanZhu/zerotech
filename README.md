# Zero Tech Website

Production-ready, minimalist company site for Zero Tech.

## Live

- Website: https://zerotech.info
- Status/Hosting: Vercel (auto-deploy from `main`)

## What's Included (current version)

- Pure static stack: HTML + CSS + Vanilla JS
- Hero counters animation limited to Hero section; supports K+, M, and + suffixes
- Traction metrics: 215K+, 3.8M, 131K+; MRR card `$5K`
- Team bios updated (Hanna CEO; Alex CMO, creator 60K subs, 3M+ views)
- Navigation: Vision, Products, Why Now, Traction, Team, Contact
- Footer: Investor Relations, Terms of Use, Privacy Policy, then social links (LinkedIn/X/YouTube/TikTok)
- Favicon: `Assets/ZeroTechLogo.png` (also Apple Touch Icon)
- Legal pages: `terms.html`, `privacy.html`
- SEO: comprehensive meta tags, Open Graph, Twitter, JSON‑LD (Organization, WebSite, BreadcrumbList), `robots.txt`, `sitemap.xml`
- Product positioning: Zero Animate (AutoAE), Zero Portfolio (Corrra), Zero Studio (coming soon)
- Product names styled with brand purple (#8c52ff) matching AutoAE logo

## Project Structure

```
ZeroComp/
├── index.html       # Main site
├── styles.css       # Styles
├── script.js        # Interactions & counter animation
├── Assets/          # Images, media (Hero.gif, logos, profiles)
├── terms.html       # Terms of Use
├── privacy.html     # Privacy Policy
├── robots.txt       # Robots directives
├── sitemap.xml      # Sitemap
└── vercel.json      # Vercel config
```

## Local Preview

Just open `index.html` in a browser, or run a simple server:

```bash
python3 -m http.server 8002
```

## Deploy (Vercel)

1. Connect repo in Vercel → Framework: Other → Root: `./`
2. `vercel.json` uses `rewrites` (no `routes`) and sets security headers
3. Auto-deploy on push to `main`

### Custom Domain (zerotech.info)

Add DNS at your registrar:

```
A     @    76.76.19.61
CNAME www  cname.vercel-dns.com
```

Or switch nameservers to:

```
ns1.vercel-dns.com
ns2.vercel-dns.com
```

## Content Editing

- Update copy/components in `index.html`
- Styles in `styles.css`; keep variables and breakpoints
- JS behavior in `script.js` (`animateCounters`) – currently scoped to `.hero-stats .stat-number`

## Contacts

- Email: hanna@zerothe.pro
``` 