# AzFIT Client Portal

Elite training platform for fitness coaches. Built with React 19, TypeScript, Vite, Tailwind CSS, and shadcn/ui.

## Features

- **Landing Page** — Dark-themed marketing site with 8 sections
- **Authentication** — Login with demo mode (auto-filled credentials)
- **Trainer Dashboard** — KPI cards, sparklines, today's schedule, alerts, client grid
- **Calendar** — 4 views (Week/Day/Month/Agenda), drag & drop, time grid
- **Program Library** — 50+ training methods, search, filter by category, match scoring
- **All-in-One Program Creator** — Full program builder with 8 steps: Goal, Method, Context, Phases, Split, Exercises, Preview, Save
- **Client Profile** — 13-tab system with metrics, progress charts, photos
- **Nutrition Hub** — TDEE calculator, macro rings, meal planner
- **Progress Photos** — Upload, gallery, before/after comparison
- **Settings** — 7-section preferences
- **AI Chat** — Floating assistant panel with quick actions

## Tech Stack

| Technology | Version |
|------------|---------|
| React | 19 |
| TypeScript | 5.7 |
| Vite | 7.2.4 |
| Tailwind CSS | 3.4.19 |
| shadcn/ui | latest |
| Framer Motion | 12 |
| Recharts | 2.15 |
| Zustand | 5 |
| React Router DOM | 7 |

## Getting Started

### Prerequisites

- Node.js 20+ and npm

### Install & Run

```bash
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

### Demo Login

- Email: `trainer@azfit.com`
- Password: `password`
- Or click **Demo Mode** on the login page

### Build for Production

```bash
npm run build
```

Output goes to `dist/` — deploy these files to your static host.

## Project Structure

```
src/
  App.tsx                 — Main routes
  store.ts                — Zustand auth store
  main.tsx                — Entry point
  types/                  — TypeScript types
  pages/                  — Page components (one per route)
  components/
    Layout.tsx            — Sidebar + top bar + AI chat
    Navbar.tsx            — Landing page navigation
    AiChat.tsx            — Floating AI assistant
    ui/                   — shadcn/ui components
  hooks/                  — Custom hooks
public/                   — Static assets (logos, images)
```

## Deployment

1. Build: `npm run build`
2. Deploy the `dist/` folder contents to your static hosting (Netlify, Vercel, GitHub Pages, etc.)
3. Ensure SPA routing is configured (all routes → index.html)

## License

MIT
