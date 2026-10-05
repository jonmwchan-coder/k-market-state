# Market State — iPad touch dashboard

A lightweight static PWA for live market-state tracking:

- HTF Trend
- Regime
- Current Leg
- Lean
- Automatic summary at the top
- Tap selected choice again to neutralize that row
- Saves state locally on the device
- Works offline after first successful load
- Can be added to the iPad Home Screen

## Run locally

From this folder:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy on Vercel

This app is plain static HTML/CSS/JS, so no build step is required.

1. Put this folder in a GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Framework preset: **Other**.
4. Leave Build Command blank.
5. Leave Output Directory as `.`.
6. Deploy.

## iPad setup

1. Open the deployed site in Safari.
2. Tap Share.
3. Tap **Add to Home Screen**.
4. Launch it from the Home Screen for the app-style full-screen view.

## State storage

The current state is stored in Safari/local app storage on that device. There is no account or backend.

If you later want the same live state synced between iPad and desktop, add a small backend such as Supabase or Firebase.
