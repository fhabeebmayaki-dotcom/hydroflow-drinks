# HYDROFLOW — Performance Hydration Brand Site (Demo)

A bold, scroll-driven brand site for a drinks company, modeled on the HYDROFLOW concept reel: a sticky product stage where the hero drink appears to **rotate as you scroll**, giant outline typography, four flavor color themes, a live nutrition label and a subscribe-and-save flow.

**Live structure:** `index.html` (everything — CSS + JS embedded) + `images/` (4 real drink photos). No build step, no dependencies. Open `index.html` or deploy the folder to any static host.

## Features

- **Scroll-rotation stage** — a 4-screen-tall scroll journey: the product photo crossfades through all 4 flavors while the card rotates (−9° to +9°), scales and drifts with scroll progress. Headline, background mega-word, flavor name and the **entire page accent color** change per stage. Clickable progress dots jump between stages.
- **Flavor lineup** — 4 flavor cards with nutrition mini-stats and a "Set the vibe" button that re-skins the page accent live.
- **Live Nutrition Facts panel** — styled like a real label; switching flavors swaps calories, sodium, carbs, potassium, magnesium and B12 instantly.
- **Subscribe & Save** — 12-pack / 24-pack plan toggle with live price math (15% subscription discount, per-can price), validated signup form (name, email, flavor, frequency) and a personalized success summary.
- **FAQ accordion** — smooth open/close, one of the sections from the original concept.
- Animated marquee, scroll reveals, giant outlined "HYDRO" footer wordmark, fully responsive with mobile nav.

## Make it yours (buyer customization)

- **Flavors:** everything is driven by the `FLAVORS` array at the top of the `<script>` — name, photo, accent color, stage headline, background word, tasting notes and all nutrition values. The stage, grid, nutrition label and subscribe form rebuild themselves from it. Add or remove flavors freely.
- **Product shots:** replace the files in `images/` (portrait orientation works best for the stage) or update the `img` paths in `FLAVORS`.
- **Pricing:** pack prices and the 15% discount live in the `PLANS` object and `paintPlan()` in the "SUBSCRIBE" script section.
- **Brand:** the wordmark is plain text in the nav/footer; the accent default is `--accent` in `:root`.

## Tech

Vanilla HTML/CSS/JavaScript in one file. Fonts: Archivo Black + Space Grotesk (Google Fonts). Photos: Unsplash (free to use). The subscribe form is a front-end demo — wire it to Shopify/Stripe/your ESP to take real subscriptions.
