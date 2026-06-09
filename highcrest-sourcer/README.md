# Highcrest Deal Sourcer

AI-powered company sourcing tool for Highcrest Management.

## Deploy to Vercel (10 minutes)

### Step 1 — Upload to GitHub
1. Go to github.com and create a new repository called `highcrest-sourcer`
2. Upload all files in this folder (index.html, api/source.js, vercel.json)

### Step 2 — Deploy on Vercel
1. Go to vercel.com and sign up / log in (free)
2. Click "Add New Project"
3. Import your GitHub repo
4. Click Deploy — Vercel auto-detects everything

### Step 3 — Add your API key (keeps it secret)
1. In Vercel, go to your project → Settings → Environment Variables
2. Add a new variable:
   - Name: `ANTHROPIC_API_KEY`
   - Value: your Anthropic API key (from console.anthropic.com)
3. Click Save, then go to Deployments and click "Redeploy"

### Step 4 — Share
Your site will be live at `https://highcrest-sourcer.vercel.app` (or similar).
Share that URL with your team — the API key stays hidden on the server.

## Cost estimate
Each search runs ~$0.10–$0.30 in API costs depending on results count.
10 searches/day ≈ ~$30–90/month.

## Files
- `index.html` — the full frontend UI
- `api/source.js` — serverless function that proxies the Anthropic API (key stays secret)
- `vercel.json` — routing config
