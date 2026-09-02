# 💰 Money Manager — Monthly Expense Tracker

A polished, offline-first monthly expense tracker built with HTML, CSS, and vanilla JavaScript. Runs entirely in the browser with `localStorage` persistence — no server needed.

## Features

- **Color-coded categories** — 8 categories with distinct colors for quick visual scanning
- **Budget limits** — per-category and overall monthly budget settings
- **Unplanned expense warnings** — flag expenses as planned or unplanned with visual warnings
- **localStorage** — all data persists in the browser, no backend required
- **Indian Rupees (₹)** — all amounts displayed in ₹ with proper INR formatting
- **Dashboard** — real-time summary cards, category spending bars, and warning banners
- **Export** — download your transactions as a CSV file

## Categories

| Category | Color |
|---|---|
| Food & Dining | 🔴 Red |
| Transport | 🔵 Blue |
| Housing & Utilities | 🟣 Purple |
| Entertainment | 🟢 Green |
| Healthcare | 🟡 Amber |
| Education | 🩷 Pink |
| Shopping | 🟠 Orange |
| Others | ⚪ Gray |

## Data Persistence

All data is stored in the browser's `localStorage` under the key `moneyManagerData`. Clearing browser data will reset all expenses. To back up your data, use the **Export** button to download a CSV file.

## Technologies

- HTML5
- CSS3 (with CSS custom properties)
- Vanilla JavaScript (ES6+)
- Font Awesome 6 (icons)
- Inter font (Google Fonts)
