 What's Fare Is Fair — Fare Comparison Web App

A responsive React.js single-page application that compares ride-hailing fares
(Ola, Uber, Rapido, InDrive) across common routes, so users can pick the
cheapest and fastest option.

## Features
- Route selection with form validation
- Live fare comparison cards with a "Best Price" badge
- Booking confirmation modal
- Multi-tab dashboard (Recent Trips, Saved Routes, Payment Methods)
- Client-side routing with React Router

## Tech Stack
- React.js (Hooks: `useState`)
- React Router DOM
- Vite (build tool)
- Plain CSS (component-scoped class names)

## Getting Started

```bash
npm install
npm run dev
```

Then open the local URL Vite prints (usually `http://localhost:5173`).

## Project Structure
```
src/
  components/    # RouteSelector, FareCard, BookingModal, Dashboard
  pages/         # Home (main comparison flow)
  data/          # Mock fare data + fare generation logic
  App.jsx        # Routing + layout
  main.jsx       # App entry point
```

## Notes
Fare data is currently mocked with a deterministic generator (`fareData.js`)
so results are consistent per route/provider. In a production version this
would be replaced by real pricing APIs from each provider.
