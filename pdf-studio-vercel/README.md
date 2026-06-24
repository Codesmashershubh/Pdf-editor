# PDF Studio — Free Browser-Based PDF Editor

A fully free, browser-based PDF editor. No backend, no database, no API keys.  
All PDF processing happens client-side using PDF.js and pdf-lib.

---

## Project Structure

```
pdf-studio/
├── index.html      ← The entire application (single file)
├── vercel.json     ← Vercel deployment configuration
└── README.md       ← This file
```

---

## Deploy to Vercel (3 ways)

### Option 1 — Vercel CLI (fastest)

```bash
# Install Vercel CLI (one-time)
npm install -g vercel

# Inside the project folder
cd pdf-studio
vercel

# Follow the prompts:
#   Set up and deploy? → Y
#   Which scope? → your account
#   Link to existing project? → N
#   Project name? → pdf-studio (or anything)
#   In which directory is your code? → ./
#   Want to override settings? → N
```

Your live URL is printed instantly. Run `vercel --prod` to promote to production.

---

### Option 2 — GitHub + Vercel Dashboard (recommended for teams)

1. Push this folder to a GitHub repo:
   ```bash
   git init
   git add .
   git commit -m "initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/pdf-studio.git
   git push -u origin main
   ```

2. Go to [vercel.com/new](https://vercel.com/new) and click **"Import Git Repository"**

3. Select your repo → click **Deploy**

4. Vercel auto-detects it as a static site.  
   - Framework Preset: **Other**  
   - Build Command: *(leave blank)*  
   - Output Directory: `.`  
   - Install Command: *(leave blank)*

5. Click **Deploy** — done in ~10 seconds.

Every future `git push` auto-deploys.

---

### Option 3 — Drag & Drop (no CLI, no Git)

1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag the entire `pdf-studio` folder into the browser window
3. Vercel deploys it instantly — no configuration needed

---

## Cost

| Resource        | Cost       |
|----------------|------------|
| Vercel Hosting  | Free (Hobby plan) |
| PDF.js CDN      | Free (cdnjs / Cloudflare) |
| pdf-lib CDN     | Free (cdnjs / Cloudflare) |
| Google Fonts    | Free       |
| **Total**       | **$0**     |

Vercel's free Hobby plan includes:
- Unlimited personal projects
- 100 GB bandwidth / month
- Automatic HTTPS / SSL
- Global CDN
- Custom domain support

---

## Custom Domain (optional, free)

1. In Vercel Dashboard → your project → **Settings → Domains**
2. Add your domain (e.g. `pdfstudio.yourdomain.com`)
3. Update your DNS with the CNAME record Vercel provides
4. HTTPS is provisioned automatically

---

## Features

- ✅ Open & view PDF files
- ✅ Edit existing text in PDFs (click any text with Select tool)
- ✅ Add new text annotations
- ✅ Freehand drawing & highlighting
- ✅ Eraser tool
- ✅ Merge multiple PDFs
- ✅ Delete individual pages
- ✅ Extract a single page as a new PDF
- ✅ Zoom in / out
- ✅ Page thumbnails panel
- ✅ Download edited PDF
- ✅ Keyboard shortcuts
- ✅ Drag & drop file open
- ✅ Works on mobile

---

## Libraries Used

| Library   | License | Version |
|-----------|---------|---------|
| [PDF.js](https://mozilla.github.io/pdf.js/) (Mozilla) | Apache 2.0 | 3.11.174 |
| [pdf-lib](https://pdf-lib.js.org/) | MIT | 1.17.1 |
| [Inter](https://rsms.me/inter/) (Google Fonts) | OFL-1.1 | — |

All served from [cdnjs.cloudflare.com](https://cdnjs.cloudflare.com) — no npm install required.
