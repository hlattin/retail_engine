# 👗 FashionStore — Virtual Try-On E-Commerce

A modern fashion e-commerce platform with AI-powered virtual try-on and a Claude-powered shopping assistant chatbot.

## Tech Stack

- **Frontend:** Next.js 14 (App Router) + Tailwind CSS
- **Auth:** Clerk
- **Database:** Supabase (PostgreSQL)
- **Storage:** Cloudflare R2
- **Payments:** Stripe
- **AI Chatbot:** Anthropic Claude API
- **Try-On:** Fashn.ai API
- **Hosting:** Vercel

## Project Structure

```
fashion-store/
├── app/                        # Next.js App Router pages
│   ├── layout.js               # Root layout (Navbar, Footer, ChatWidget)
│   ├── page.js                 # Homepage (Hero, Featured Products)
│   ├── shop/page.js            # Catalog page with filters
│   ├── product/[id]/page.js    # Product detail + Try-On button
│   ├── cart/page.js            # Cart & checkout
│   └── auth/login/page.js      # Login / Signup
│
├── components/
│   ├── layout/
│   │   ├── Navbar.jsx          # Top nav with cart, search, auth
│   │   ├── Footer.jsx          # Footer + newsletter
│   │   └── Sidebar.jsx         # Mobile nav drawer
│   ├── ui/                     # Reusable base components
│   │   ├── Button.jsx
│   │   ├── Badge.jsx
│   │   ├── Modal.jsx
│   │   └── Spinner.jsx
│   ├── catalog/
│   │   ├── HeroBanner.jsx      # Homepage hero
│   │   ├── CategoryBanner.jsx  # Category tiles
│   │   ├── ProductCard.jsx     # Product tile
│   │   ├── ProductGrid.jsx     # Responsive grid
│   │   └── FilterPanel.jsx     # Style/price/size filters
│   ├── chatbot/
│   │   ├── ChatWidget.jsx      # Floating chat window
│   │   ├── ChatMessage.jsx     # Message bubble
│   │   └── ChatInput.jsx       # Input + send
│   └── tryon/
│       ├── PhotoUpload.jsx     # Upload user photo
│       ├── TryOnModal.jsx      # Full try-on flow
│       └── TryOnResult.jsx     # Result display
│
├── hooks/
│   ├── useCart.js              # Cart state management
│   ├── useChat.js              # Chat + Claude API
│   └── useTryOn.js             # Try-on + Fashn.ai API
│
├── lib/
│   ├── api.js                  # API helpers
│   ├── utils.js                # Utility functions
│   └── constants.js            # App constants
│
├── data/
│   ├── products.js             # Mock products (swap for DB later)
│   └── categories.js           # Mock categories
│
└── public/images/              # Static assets
```

## Getting Started

```bash
npm install
npm run dev
```

Visit `http://localhost:3000`

## Environment Variables (.env.local)

```env
ANTHROPIC_API_KEY=
FASHN_API_KEY=
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
STRIPE_SECRET_KEY=
```

## Build Phases

- [x] Phase 1 — Project structure
- [ ] Phase 2 — Storefront & catalog UI
- [ ] Phase 3 — AI chatbot integration
- [ ] Phase 4 — Virtual try-on integration
- [ ] Phase 5 — Auth, cart & checkout
- [ ] Phase 6 — Database & real product data# retail_engine
Clothing store 
