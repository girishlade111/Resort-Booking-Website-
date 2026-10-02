# Dandeli Adventure Resorts — Resort Booking Website

A full-featured resort booking website for **Dandeli Adventure Resorts** — browse rooms, explore activities, check availability, and walk through a complete client-side booking flow (search → room selection → guest details → payment form → OTP step → confirmation). Built with **Vite + React 18 + TypeScript**, styled with **Tailwind CSS** and **shadcn/ui**, animated with **Framer Motion**.

This is a static, client-side demo site: the booking/payment steps are a realistic UI flow with no real backend — no charges are made.

---

## Features

- **Multi-page experience** — Home, Accommodation, Activities, Gallery, About, Contact, Booking, Booking Success, 404
- **Room discovery** — room cards, search/filter form, featured listings
- **End-to-end booking flow** — date + guest selection, personal info, mock payment form, OTP input, booking confirmation
- **Activities & attractions** — activity cards, featured activities, nearby-attractions section
- **Engagement widgets** — chatbot, WhatsApp button, ad popup, promo/discount banners, special offers
- **Polish** — dark/light theme support, scroll-to-top, tilt cards, toasts, fully responsive layout

## Tech Stack

- **Build:** Vite 6, TypeScript
- **UI:** React 18, react-router-dom, Tailwind CSS, shadcn/ui (Radix primitives), Framer Motion, lucide-react
- **Forms:** react-hook-form, zod validation
- **Dates:** date-fns, react-day-picker

## Quick Start

```bash
npm install --legacy-peer-deps
npm run dev        # http://localhost:5173
```

## Project Structure

```
src/
├── pages/            # Index, Accommodation, Activities, Booking, BookingSuccess, Gallery, About, Contact, NotFound
├── components/       # Navbar, Hero, RoomCard, SearchForm, BookingForm, PaymentForm, OtpInput, ChatBot, ...
│   └── ui/           # shadcn/ui primitives
├── hooks/            # theme, mobile, toast
└── lib/              # utils
public/               # static assets, favicon, og-image
```

## Build & Deploy

```bash
npm run build        # outputs to dist/
```

Static output — deploy anywhere static files are served:

- **Cloudflare Pages:** `cloudflare pages_deploy resort-booking-website- dist`
- **GitHub Pages / Netlify / Vercel:** point at `dist/` (SPA — add a `/* /index.html 200` redirect rule)

## Environment Variables

None — the site is fully client-side and needs no API keys or backend.

---

Built by **Girish Lade** — [ladestack.in](https://ladestack.in)
