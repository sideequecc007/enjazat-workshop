# Al Enjazat Workshop ERP — Deployment Guide

## What's in this folder

```
enjazat-erp/
├── index.html          ← Website entry point
├── package.json        ← Project config
├── vite.config.js      ← Build tool config
├── vercel.json         ← Vercel deployment config
├── .gitignore          ← Files to exclude from GitHub
└── src/
    ├── App.jsx         ← Your full ERP (6,539 lines)
    └── main.jsx        ← React entry point
```

---

## STEP 1 — Create a GitHub Account (skip if you have one)

1. Go to https://github.com
2. Click **Sign up**
3. Enter your email, create a password, choose a username (e.g. `enjazat`)
4. Verify your email

---

## STEP 2 — Create a New Repository on GitHub

1. After logging in, click the **+** button (top right) → **New repository**
2. Repository name: `enjazat-erp`
3. Set to **Public** (required for free Vercel)
4. Click **Create repository**
5. You'll see an empty repo page — keep it open

---

## STEP 3 — Upload your files to GitHub

1. On your new empty repo page, click **uploading an existing file** (link in the middle)
2. Drag and drop ALL files from the `enjazat-erp` folder:
   - `index.html`
   - `package.json`
   - `vite.config.js`
   - `vercel.json`
   - `.gitignore`
   - The entire `src` folder (drag the folder itself)
3. Scroll down, type commit message: `Initial upload — ERP v11`
4. Click **Commit changes**

---

## STEP 4 — Deploy to Vercel (free)

1. Go to https://vercel.com
2. Click **Sign Up** → choose **Continue with GitHub**
3. Authorize Vercel to access your GitHub
4. Click **Add New Project**
5. Find `enjazat-erp` in the list → click **Import**
6. Vercel auto-detects Vite — settings are pre-filled ✅
7. Click **Deploy**
8. Wait ~2 minutes for the build to complete

---

## STEP 5 — Get your live URL

After deployment, Vercel shows:
> 🎉 **Congratulations! Your site is live.**
> URL: `https://enjazat-erp.vercel.app`

Click the URL — your ERP is live!

---

## STEP 6 — Custom URL (Optional)

To change the URL from the auto-generated name:
1. In Vercel dashboard → your project → **Settings** → **Domains**
2. Click **Edit** next to the auto-generated name
3. Change to something like `enjazat-workshop`
4. Your URL becomes: `https://enjazat-workshop.vercel.app`

---

## Future Updates

Every time you get a new version of the ERP from Claude:
1. Go to your GitHub repo
2. Click on `src/App.jsx`
3. Click the ✏️ pencil (Edit) icon
4. Delete all content, paste new ERP code
5. Click **Commit changes**
6. Vercel **auto-rebuilds and deploys** in ~2 minutes

---

## Important Notes

- ✅ **Free forever** — GitHub Free + Vercel Hobby plan
- ✅ **No credit card needed**
- ⚠️ **Data resets on page refresh** — this is in-memory only (v11)
- ⚠️ **Anyone with the link can use it** — no login protection yet
- 🔒 For password protection, upgrade to Vercel Pro ($20/mo) or wait for v12 with Supabase login

---

*Al Enjazat Technical Works · ERP v11 · Doha, Qatar*
