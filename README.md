StockSense — Inventory Management

A single-page inventory management app: products, receipts, delivery orders, internal transfers, stock adjustments, and a full move-history ledger.

Running it

This is a single self-contained index.html file — no build step, no dependencies to install.

Locally: double-click index.html, or run a tiny local server (python3 -m http.server) and open it in your browser.
On GitHub Pages: once this repo is pushed to GitHub, enable Pages in the repo settings (see below) and it's live at https://<your-username>.github.io/<repo-name>/.
Data storage

All data (products, stock levels, documents, ledger) is saved in the browser's localStorage. That means:

Data is per-browser, per-device — it doesn't sync between people or devices.
Clearing site data / browsing data for this page will reset it back to the seed demo data.
There is no backend or database; this is a front-end demo/prototype.
AI guide

The app includes an "Ask the StockSense guide" chat button. It only works when opened from its original claude.ai artifact link — it depends on a live connection back to Claude that isn't available once the page is hosted elsewhere (GitHub Pages, a local file, etc.). Outside that environment, the button still appears but the chat will explain it can't connect and point the user to the sidebar instead. Everything else in the app works fully standalone.

Installing as an app (PWA)

On supported browsers (Chrome/Edge on desktop or Android), an "Install app" button appears in the top bar, adding a home-screen/desktop icon. On iOS Safari, use Share → "Add to Home Screen" instead.
