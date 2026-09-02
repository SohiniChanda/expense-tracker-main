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

## Deployment to GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `money-manager` (or any name you prefer)
3. Choose **Public** (required for free Pages) or **Private**
4. Do NOT initialize with README — we already have the files
5. Click **Create repository**

### Step 2 — Push your code

Open a terminal in the `expense-tracker` folder and run:

```bash
git remote add origin https://github.com/YOUR_USERNAME/money-manager.git
git branch -M main
git add .
git commit -m "feat: monthly expense tracker with color-coded categories, budgets, and localStorage"
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: `main`, folder: `/ (root)`
5. Click **Save**
6. Your site will be live at `https://YOUR_USERNAME.github.io/money-manager/`

### Alternative: One-command deploy via GitHub CLI

```bash
gh repo create money-manager --source=. --remote=origin --public --push
```

Then enable Pages in the repo settings as above.

## Alternative Hosting Options

| Platform | How |
|---|---|
| **Netlify** | Push to GitHub → [app.netlify.com](https://app.netlify.com) → Import repo → Deploy |
| **Vercel** | Push to GitHub → [vercel.com](https://vercel.com) → Import → Deploy |
| **Cloudflare Pages** | Push to GitHub → Cloudflare Dashboard → Pages → Connect repo |

All of these auto-deploy on every `git push`.

## Local Usage

Simply open `index.html` in any modern browser — no build step or server required.

To test locally with a server:

```bash
# Python 3
python -m http.server 8080

# Node.js (npx)
npx serve .
```

Then open `http://localhost:8080`.

## Data Persistence

All data is stored in the browser's `localStorage` under the key `moneyManagerData`. Clearing browser data will reset all expenses. To back up your data, use the **Export** button to download a CSV file.

## Technologies

- HTML5
- CSS3 (with CSS custom properties)
- Vanilla JavaScript (ES6+)
- Font Awesome 6 (icons)
- Inter font (Google Fonts)
