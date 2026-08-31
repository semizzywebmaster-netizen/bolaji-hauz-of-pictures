# BOLAJI HAUZ OF PICTURES (BHP) - Cloudflare Pages Deploy Package

This zip is ready to deploy to https://bolaji-hauz-of-pictures.pages.dev

## What's Inside
- index.html -> Your full multi-page site (Home, About, Services, Portfolio, Equipment, Pricing, Gallery, Blog, Contact, Admin + AI Bot)
- _redirects -> SPA routing fix for Cloudflare Pages (/* /index.html 200)
- _headers -> Security & caching headers
- wrangler.toml -> Cloudflare config
- assets/ -> Your BHP logo and founder photo

## Business Info (Locked)
- Business: BOLAJI HAUZ OF PICTURES (BHP)
- Photographer: Bolaji Emmanuel Ayodeji
- Phone/WhatsApp: 08141317088 (+2348141317088)
- Email: boladeji89@gmail.com
- Address: 15, Olorun Esan, Adigbe, Ogun State, Nigeria

## Admin Access
- URL: /admin/login or /#/admin/login (hash routing)
- Username: bolaji_admin
- Password: BHPadmin2026!
- Auth: localStorage token bhp_admin_token with 24h expiry
- Manage: Site Settings, Services, Portfolio (upload from device -> base64), Testimonials (Nigerian), Equipment, Bookings (export CSV), Gallery PIN, Deploy guide

## AI Bot
- Bottom-left "Ask BHP AI" - only answers photography, camera accessories, BHP services
- Quick chips: Wedding packages, Portrait prices, Best lens, Book session, Equipment list, WhatsApp

## Deploy Option 1: Cloudflare Pages Dashboard (Easiest - Recommended)
1. Go to https://dash.cloudflare.com -> Pages -> Create a project -> Direct Upload
2. Drag & Drop this entire folder or zip
3. Project name: bolaji-hauz-of-pictures
4. Deploy -> Your site will be live at bolaji-hauz-of-pictures.pages.dev
5. Custom domain: Add bolajihauzofpictures.com if you have it

## Deploy Option 2: Wrangler CLI
```bash
npm install -g wrangler
wrangler pages publish ./ --project-name=bolaji-hauz-of-pictures
```

## Deploy Option 3: GitHub -> Pages (CI)
1. Create GitHub repo, push this folder
2. Cloudflare Dashboard -> Pages -> Create project -> Connect to Git
3. Build settings:
   - Framework: None (static)
   - Build command: (leave empty)
   - Output directory: /
4. Deploy

## After Deploy
- Test: /admin/login with bolaji_admin / BHPadmin2026!
- Go to Portfolio Manager -> "Load 12 Nigerian Starter Portfolio" OR upload your real client work via "Upload from device"
- Test AI Bot bottom-left, WhatsApp floating bottom-right -> wa.me/2348141317088
- All data is stored in browser localStorage (bhp_portfolio, bhp_bookings, etc) - no backend needed. For real backend, connect to Cloudflare KV/D1 later.

## Features
- Multi-page client router (no page reload)
- Luxury black/charcoal/gold design
- Real images, Nigerian testimonials
- Booking form with BHP-XXXX-2026 reference ID
- Client gallery PIN: BHP2026
- SEO: LocalBusiness JSON-LD, meta for Ogun/Abeokuta/Adigbe photographer

## Support
WhatsApp: +2348141317088
Email: boladeji89@gmail.com
