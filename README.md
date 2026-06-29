# Empty Reuse — UX/UI Case Study

A single-page, self-contained case study for **Empty Reuse**, the field-facing mobile app in the MATCHLOG logistics platform. The app matches empty import containers to nearby export demand (a "street turn"), cutting empty miles, fuel and CO₂ while turning idle assets into revenue.

Built as a static site — plain HTML, CSS and a few lines of vanilla JS. No build step, no dependencies.

## Preview

Open `index.html` in any browser, or serve it locally:

```bash
# Python
python3 -m http.server 8000
# then visit http://localhost:8000

# or Node
npx serve .
```

## Structure

```
empty-reuse-case-study/
├── index.html            # the case study (references images in /assets)
├── assets/               # in-app screenshots used throughout the page
│   ├── dashboard.jpg
│   ├── empty-reuse-list.jpg
│   ├── reuse-detail-containers.jpg
│   ├── reuse-detail-payments.jpg
│   ├── add-request-step1.jpg
│   ├── add-request-details.jpg
│   ├── payment-charges.jpg
│   ├── payment-success.jpg
│   └── color-palette.jpg
├── boards/               # the same case study exported as numbered image
│   ├── 01_...jpg         # boards (3000px wide) for Behance / Dribbble
│   └── ... 13_...jpg
├── README.md
└── .gitignore
```

## Case study outline

The narrative follows a Situation → Task → Action → Result structure:

1. **Cover** — hero with app screens
2. **Project & Challenge**
3. **Situation** — two empty trips that should have been one
4. **Research** — Field Coordinator & Shipping-Line Approver, the reuse journey
5. **Task** — run a reuse from your pocket
6. **Information Architecture** — the five-step spine and status model
7. **Wireframes** — thumb-first low-fidelity
8. **Action** — Dashboard · Add Request · Match & Details · Approval & Payment, each with design decisions
9. **Design system** — the blue colour ramp, status chips, components
10. **Result** — the savings impact

## Tech

- Plain HTML + CSS (CSS custom properties, Grid/Flexbox)
- Vanilla JS for scroll progress and reveal-on-scroll (respects `prefers-reduced-motion`)
- Fonts: Plus Jakarta Sans + Inter via Google Fonts
- Fully responsive, no framework

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Choose `main` / root, save. The site publishes at `https://<user>.github.io/<repo>/`.

## Notes

Product UI shown is the live Empty Reuse mobile app; sample IDs, customers and amounts are illustrative. Result figures reflect the in-app savings dashboard.

---

© 2026 · Designed by a Senior UI/UX Designer. Case study for portfolio use.
