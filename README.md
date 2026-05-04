# BetLedger

Local-first PWA for tracking friendly bets between a couple or group of friends.

## Features

- Add players
- Top up user credits
- Create open bets before results are known
- Settle bets by winner and loser(s)
- Track money balances and non-money prizes/favors/items
- Open, settled, and cancelled bet history
- Calendar-style settlement view
- Light/dark mode
- Export JSON backup
- Offline PWA support through service worker
- Local browser storage only; no backend required

## Run locally

Open `index.html` directly in a browser, or serve the folder locally for full PWA/service worker behavior:

```bash
python3 -m http.server 5173
```

Then open:

```text
http://localhost:5173
```

## Deploy

This can be deployed to GitHub Pages, Netlify, Vercel, or any static host.

For GitHub Pages:

1. Push this folder to a repo named `betledger`.
2. Go to Settings → Pages.
3. Source: Deploy from branch.
4. Branch: `main`, folder `/root`.

## Important

Data is stored in `localStorage`, so it is tied to the device/browser. For multi-device sync or shared group access, migrate storage to Firebase, Supabase, or another backend.
