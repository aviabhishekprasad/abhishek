# GitHub Pages Deployment Guide
## Abhishek Prasad — Personal Portfolio

---

## Files to Upload
```
portfolio/
├── index.html
├── style.css
├── script.js
├── cv.pdf                  ← your CV PDF
├── avi_full.jpg            ← full body photo
└── avi_headshot.jpg        ← headshot / portrait photo
```

---

## Step-by-Step Deployment

### 1. Create a GitHub Account
Go to https://github.com and sign up (free).

### 2. Create a New Repository
- Click the **"+"** icon → **"New repository"**
- Repository name: `abhishek-prasad` (or your preferred name)
- Set to **Public**
- Do NOT initialize with README
- Click **"Create repository"**

### 3. Upload Your Files
**Option A — Via GitHub Web Interface (easiest):**
1. Open your new repository
2. Click **"uploading an existing file"** or **"Add file → Upload files"**
3. Drag and drop all 6 files listed above
4. Click **"Commit changes"**

**Option B — Via Git CLI:**
```bash
cd your-portfolio-folder
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/abhishek-prasad.git
git push -u origin main
```

### 4. Enable GitHub Pages
1. Go to your repository → **Settings**
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **"Deploy from a branch"**
4. Branch: **main**, Folder: **/ (root)**
5. Click **Save**

### 5. Access Your Site
After 1–2 minutes, your site will be live at:
```
https://YOUR_USERNAME.github.io/abhishek-prasad/
```

---

## Custom Domain (Optional)
If you have a domain like `abhishekprasad.com.np`:
1. In repository Settings → Pages → Custom domain, enter your domain
2. Add a CNAME DNS record pointing to `YOUR_USERNAME.github.io`

---

## Updating Your Portfolio
To update content, simply edit the HTML files and push/upload again. Changes go live within minutes.

---

## Tips
- The `cv.pdf` file must be in the **same folder** as `index.html` for the download button to work
- Image files (`avi_full.jpg`, `avi_headshot.jpg`) must also be in the **root folder**
- GitHub Pages is completely **free** for public repositories
