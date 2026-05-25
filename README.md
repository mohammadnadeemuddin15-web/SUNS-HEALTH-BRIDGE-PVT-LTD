# 🏥 Suns Health Bridge — Business Management System

A complete financial management system for medical device import businesses.
Built with React. Free to host on Vercel.

---

## Features

- 📊 **Dashboard** — Revenue, outstanding, low-stock alerts at a glance
- 📋 **Quotations** — Create quotations, convert to invoices in one click
- 🧾 **Invoices** — Full invoice tracking with balance and overdue detection
- 📦 **Inventory** — Stock levels, reorder alerts, margin tracking
- 💳 **Payments** — Record payments, track outstanding collections
- 🏥 **Customers** — Hospital/clinic directory with revenue history

---

## Quick Start (Local Development)

### Step 1 — Install Node.js
Download from: https://nodejs.org (choose LTS version)

### Step 2 — Install dependencies
Open Terminal / Command Prompt in this folder and run:
```bash
npm install
```

### Step 3 — Start the app
```bash
npm start
```
The app opens at http://localhost:3000

---

## Deploy to Vercel (Free — Gets a public URL)

### Step 1 — Push to GitHub
1. Create account at https://github.com
2. Create new repository named `suns-health-bridge`
3. Upload all these files (drag & drop into GitHub)

### Step 2 — Deploy
1. Go to https://vercel.com
2. Sign in with GitHub
3. Click "Add New Project" → select your repository
4. Click Deploy

✅ Your app will be live at: `https://suns-health-bridge.vercel.app`

---

## Project Structure

```
suns-health-bridge/
├── public/
│   └── index.html          ← HTML shell
├── src/
│   ├── App.js              ← Main app + navigation
│   ├── index.js            ← React entry point
│   ├── data.js             ← Sample data + helper functions
│   ├── styles.js           ← Global CSS styles
│   ├── hooks/
│   │   └── useLocalStorage.js  ← Data persistence hook
│   ├── components/
│   │   └── Badge.js        ← Status badge component
│   └── pages/
│       ├── Dashboard.js    ← Dashboard page
│       ├── Quotations.js   ← Quotations page
│       ├── Invoices.js     ← Invoices page
│       ├── Inventory.js    ← Inventory page
│       ├── Payments.js     ← Payments page
│       └── Customers.js    ← Customers page
└── package.json            ← Project configuration
```

---

## Upgrading to Team-Shared Data (Optional)

Currently data is stored in each browser's localStorage.
To share data across team members, connect Firebase:

1. Create free account at https://firebase.google.com
2. Create a Firestore database
3. Replace `useLocalStorage` hook with Firebase reads/writes

Contact your developer for this upgrade.

---

Built for Suns Health Bridge · Karachi, Pakistan
