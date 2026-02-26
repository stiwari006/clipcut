# ✂️ ClipCut — Video to Shorts

Turn long videos into viral short clips. Free for up to 10 users. Runs 100% in the browser.

---

## 🚀 Deploy to Vercel

### Option A — Vercel CLI
```bash
npm i -g vercel
cd clipcut
vercel
```

### Option B — GitHub + Dashboard
1. Push to GitHub repo
2. vercel.com → New Project → Import → **Framework: Other**
3. Click **Deploy**

---

## 👥 Multi-User & Free Tier

| Feature | Free (default) | Pro (coming soon) |
|---------|---------------|-------------------|
| Max users | **10** | Unlimited |
| Clips per export | **5** | Unlimited |
| Clip duration | **up to 60s** | Up to 90s |
| Cost | **$0** | $9/month |

- Users register via the gate screen (name + optional email)
- Session is saved in `localStorage` — returning users auto-login
- Up to 10 unique users can register; after that, existing users still work
- **All video processing is client-side** — 100+ users can use simultaneously with zero server load

## 📤 Shareable

Share your deployed URL — each person:
1. Enters their name on the gate screen
2. Processes video entirely in their own browser  
3. Downloads clips directly

Built-in share buttons: X/Twitter, WhatsApp, LinkedIn, Facebook, Telegram, Email.

---

## 📁 Structure

```
clipcut/
├── public/
│   └── index.html    ← full self-contained app
├── vercel.json       ← COOP/COEP headers for FFmpeg.wasm
├── package.json
└── README.md
```

## 🔧 Local Dev

```bash
npx serve public -p 3000
```
# clipcut
