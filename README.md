# Ledger House

A static expense ledger with a traditional counting-house illustration, an interactive abacus, and USD/CNY conversion.

## Preview locally

Run from this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://127.0.0.1:8765/ in your browser.

## Files

- `index.html`: page structure and application logic
- `styles.css`: layout and Cardo typography
- `assets/ui/`: illustrations, panels, and icons

## Data and exchange rates

Entries and currency preferences are saved in the current browser's localStorage, not shared between users. Existing entries without a currency are treated as USD. Frankfurter supplies daily reference exchange rates; the UI shows the rate date and cached/unavailable status.

## Deployment

Publish this directory with any static hosting service. No build command is required; keep `index.html`, `styles.css`, and `assets/` together.
