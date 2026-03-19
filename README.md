# RentMate Ghana 🇬🇭

> Ghana's premier zero-commission rental platform — connecting landlords and renters across all 16 regions.

---

## What It Is

RentMate Ghana is a fully self-contained, single-file web app for listing and browsing rental properties across Ghana. No backend, no database, no server costs. Just one HTML file you can host anywhere for free.

- **Renters** can search, filter, and contact landlords directly via WhatsApp
- **Landlords** can post properties for free — no signup, no commission
- **Admins** can approve, reject, and verify listings through a built-in password-protected panel

---

## Features

### User Side
- Browse listings across all 16 regions of Ghana
- Filter by region, city, property type, and max price
- Click-through region pills for quick regional browsing
- Full listing detail page with photo gallery and sidebar contact card
- Direct WhatsApp contact button (pre-filled message)
- Submit a property form with photo upload and validation

### Admin Panel
- Password-protected admin console (default: `admin123`)
- Approve, reject, verify, and unpublish listings
- Metrics dashboard: total, pending, approved, rejected counts
- Filterable table with tabs: All / Pending / Approved

### Technical
- Zero dependencies — pure HTML, CSS, JavaScript
- All 16 Ghana regions with 260+ cities pre-loaded
- Fully responsive (mobile, tablet, desktop)
- Dark luxury design with gold accent system
- Skeleton loading states, toast notifications, drag-and-drop image upload

---

## Live Demo

Deploy in 30 seconds — see [Hosting](#hosting) below.

---

## Getting Started

1. Download `index.html`
2. Open it in any browser — it works offline with no setup

That's it. No `npm install`. No config files. No terminal.

---

## Hosting (Free)

This is a static single-file site. It hosts for free on all of the following:

### Netlify Drop (easiest — 30 seconds)
1. Put `index.html` inside a folder
2. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
3. Drag the folder into the page
4. Your site is live at `yourname.netlify.app`

### GitHub Pages (recommended for permanence)
1. Create a free account at [github.com](https://github.com)
2. Create a new **public** repository named `rentmate-ghana`
3. Upload `index.html` (rename it to `index.html` if needed)
4. Go to **Settings → Pages → Branch: main → Save**
5. Live at `https://yourusername.github.io/rentmate-ghana`

### Cloudflare Pages (fastest globally)
1. Go to [pages.cloudflare.com](https://pages.cloudflare.com)
2. Create account → **Create application → Pages → Upload assets**
3. Upload `index.html` → Deploy
4. Live at `yourname.pages.dev`

> **Important:** Always name your file `index.html` before uploading, or visitors will see a directory listing instead of your site.

---

## Admin Access

Switch to the admin panel using the **⚙️ Admin** button in the bottom-right corner.

| Field    | Value      |
|----------|------------|
| Password | `admin123` |

> Change the password by editing `const ADMIN_PW = 'admin123'` in the script section of `index.html`.

---

## Customisation

All editable values are near the top of the `<script>` section:

| Variable    | What it controls                        |
|-------------|------------------------------------------|
| `ADMIN_PW`  | Admin panel password                    |
| `GH_DATA`   | All regions and their cities            |
| `listings`  | Seed/demo listing data                  |
| `IMGS`      | Fallback image URLs                     |

To change colours, edit the CSS variables in `:root` at the top of the file (e.g. `--gold`, `--obsidian`).

---

## Project Structure

```
index.html          ← entire app (HTML + CSS + JS in one file)
README.md           ← this file
```

No build step. No node_modules. No framework.

---

## Roadmap Ideas

- [ ] LocalStorage persistence (listings survive page refresh)
- [ ] WhatsApp Business API integration
- [ ] Image hosting via Cloudinary free tier
- [ ] PWA / installable app for mobile
- [ ] Ghana Mobile Money payment badge
- [ ] SMS notification via Hubtel API

---

## Contributing

1. Fork the repo
2. Edit `index.html`
3. Open a pull request

No build tools required — just save and refresh.

---

## License

MIT — free to use, modify, and deploy commercially.

---

## Credits

Built for Ghana. Hosted free. Zero commission. Always.

> *Verify in person before any payment.*
