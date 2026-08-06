# GRIND IT Stump Removal demo

Independent, offline-safe Vite demo for GRIND IT Stump Removal, LLC. The quote builder validates locally, previews selected images, and shows a transparent local success state; it does not transmit customer data.

## Install and run

```bash
cd /home/autobot-leader/grind-it-stump-removal-demo
npm install
npm run dev
```

Open `http://localhost:5177/`.

## Structure

- `index.html` — semantic page, metadata and local-business schema
- `style.css` — responsive design system and motion/accessibility rules
- `main.js` — menu, lightbox, quote steps, validation and image previews
- `public/images/` — local optimized/replacement-ready assets
- `public/robots.txt`, `public/sitemap.xml` — private-demo defaults; update for launch
- `SOURCES.md` — factual and visual provenance
- `OWNER_CONFIRMATION_NEEDED.md` — launch checklist
- `IMAGE_REPLACEMENT_GUIDE.md` — exact plan for genuine business photography

## Replace images

Add approved, optimized WebP/AVIF files to `public/images/`, preserve the documented crops, and update matching paths and alt text in `index.html`. Do not use social-media CDN URLs in production.

## Connect the quote form

Replace the `submit` handler in `main.js` with a POST to the owner's selected email form service, SMS workflow, CRM, or server endpoint. Upload files as `multipart/form-data`, add server-side validation, spam protection, consent/privacy copy, delivery logging, and a real failure state. The current demo intentionally stores and sends nothing.
