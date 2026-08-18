# Flo

A period-tracking app UI (Login, Sign up, Setup, Home, Calendar, Log Period).

## Run locally

```bash
npm install
npm run dev
```

## Deploy — GitHub + Render

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/flo-app.git
   git push -u origin main
   ```
   (Create the empty `flo-app` repo on GitHub first, without a README, then run the commands above.)

2. **Deploy on Render**
   - Go to https://dashboard.render.com → **New** → **Static Site**
   - Connect your GitHub account and select the `flo-app` repo
   - Settings:
     - **Build Command:** `npm install && npm run build`
     - **Publish Directory:** `dist`
   - Click **Create Static Site**

Render will build and give you a live URL (e.g. `https://flo-app.onrender.com`). Every push to `main` auto-redeploys.
