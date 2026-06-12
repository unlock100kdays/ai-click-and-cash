# AI Click And Cash — Project Context

## Project Overview
A high-converting VSL/sales funnel landing page for the **AI Click And Cash** product.
The angle is: **making money online with AI** — no tech skills required.

## Design Reference
- Reference page: https://www.grabjellylean.com/vsl3-ml2
- Same HTML structure, layout, CSS variables, fonts, and design system
- Images downloaded from reference page and re-hosted on Cloudflare Pages
- Copy and angle changed from weight loss → AI income

## Cloudflare Deployment
- **Account ID:** `(stored in GitHub Secret: CLOUDFLARE_ACCOUNT_ID)`
- **API Token:** `(stored in GitHub Secret: CLOUDFLARE_API_TOKEN)`
- **Project Name:** ai-click-and-cash
- **Production URL:** https://ai-click-and-cash.pages.dev
- **Latest Deployment:** https://e44a3750.ai-click-and-cash.pages.dev
- Deploy command: `CLOUDFLARE_API_TOKEN=<token> npx wrangler pages deploy . --project-name ai-click-and-cash --branch main`

## File Structure
```
AI Click And Cash/
├── CONTEXT.md                ← this file
├── index.html                ← main landing page
├── privacy-policy.html       ← Privacy Policy page
├── terms.html                ← Terms of Service page
├── refund-policy.html        ← Refund Policy page
├── earnings-disclaimer.html  ← Earnings Disclaimer page
├── anti-spam.html            ← Anti-Spam Policy page
├── dmca.html                 ← DMCA Notice page
├── contact.html              ← Contact Us page (with form)
└── images/                   ← all images (downloaded from reference)
    ├── today.webp
    ├── logosnovas.png
    ├── img-6-bottles.webp
    ├── img-3-bottles.webp
    ├── img-2-bottles.webp
    ├── hour-glass.png
    ├── ship-icon.png
    ├── cards-dark.webp
    ├── cards.webp
    ├── guarantee-badge.webp
    ├── gmp.png
    ├── fda.png
    ├── nat.png
    ├── foreign.png
    ├── gmo.png
    ├── shopping.png
    ├── 1_perfil.png / 1-corpo.jpg
    ├── 2_perfil.png
    ├── avatar.webp
    ├── 4_perfil.png / 4-corpo.jpg
    └── 10.jpg–13.jpg
```

## Tech Stack
- **Framework:** Vanilla HTML/CSS/JS (no build step)
- **CSS:** Bootstrap 5.3, Bootstrap Icons, Font Awesome 6.5
- **Fonts:** Nunito Sans, Roboto, DM Sans, Playfair Display (Google Fonts)
- **CSS Variables:** `--primary-color: #9c130d`, `--secondary-color: #fb8a69` (matches reference)
- **Hosting:** Cloudflare Pages (static deploy)

## Page Structure — index.html
1. TODAY-style header (logo + nav + sign in)
2. Hero section — headline + video placeholder (click reveals quiz)
3. 5-step quiz funnel (DM Sans / Playfair Display styled card)
4. After-quiz products section (shown by default, hidden during quiz)
5. 3 pricing tiers — `.item`, `.item.promo` (Best Value), `.kit1/2/3`
6. Guarantee section (red background, badge + text)
7. Free access banner (black background)
8. Testimonials — `.card-container` with Bootstrap stars
9. Second CTA + products repeat
10. FAQ — Bootstrap accordion (red gradient background)
11. Second guarantee repeat
12. Final CTA + products repeat
13. Footer — red background, legal nav links, disclaimer text blocks

## Legal Pages
All legal pages share the same style: red top bar with back-to-home link, clean content layout, consistent footer with cross-links.
- **privacy-policy.html** — Data collection, usage, sharing, rights
- **terms.html** — Terms of service, no income guarantee, IP, prohibited uses
- **refund-policy.html** — 60-day guarantee, how to request, processing time
- **earnings-disclaimer.html** — No income guarantee, FTC compliance, results vary
- **anti-spam.html** — CAN-SPAM compliance, unsubscribe process
- **dmca.html** — Takedown process, counter-notification, repeat infringer policy
- **contact.html** — Contact cards (support/billing/legal) + working contact form

## Product Angle
- **Product Name:** AI Click And Cash
- **Hook:** Ex-tech insider reveals the AI system that helped ordinary people earn passive income online
- **USP:** No coding, no tech skills, no experience needed — AI does the heavy lifting
- **Packages:** 3-tier access (Basic $79, Popular $69/mo, Best Value $49/mo)
- **Guarantee:** 60-day money-back guarantee
- **Support email:** support@aiclickandcash.com

## Quiz Flow
5 steps: goals → age range → experience level → income goal → obstacles
- Steps 1 & 5 are multi-select (Continue button appears after any selection)
- Steps 2, 3, 4 are single-select with auto-advance on click
- Loading screen with rotating messages → result card with profile summary + income projection
- Result CTA scrolls to product section

## Notes
- Video section is a styled placeholder (click triggers quiz)
- Testimonials use same profile images from reference page, copy rewritten for AI income angle
- Trust badges reused from reference (gmp, fda, nat, foreign, gmo)
- All footer links are live and working
