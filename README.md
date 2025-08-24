# Sinsweets — Brand Site (Vite + React + Tailwind)

A luxurious single‑page site for **sinsweets.com** with brand colors, hero, bestsellers, the 7‑Sins collection, newsletter, and footer.

## Quick start
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
npm run preview
```

## Deploy to Vercel
1. Create a new project in Vercel and import this repo.
2. Framework preset: **Vite** (defaults are fine).
3. Deploy.
4. In Vercel → **Domains**, add `sinsweets.com` and `www.sinsweets.com`.
5. Copy the DNS records Vercel shows:
   - Apex `sinsweets.com`: A/ALIAS to Vercel
   - `www`: CNAME to `cname.vercel-dns.com`
6. Set the records at your domain registrar. SSL will auto‑provision.

## Deploy to Netlify
1. New site → Import from Git.
2. Build command: `npm run build`
   Publish directory: `dist`
3. Add domain `sinsweets.com` + `www` and follow the shown DNS records.

## Notes
- Fonts: Playfair Display (serif) & Montserrat (sans) are loaded via Google Fonts in `index.html`.
- Images: Placeholder SVGs are embedded (no external calls). Replace with real product photos in `/public` and update `<img>` sources.
- To wire a real newsletter (Klaviyo/Mailchimp), connect the form action or add a simple API route.