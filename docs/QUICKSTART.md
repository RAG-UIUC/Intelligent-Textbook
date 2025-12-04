# Quick Start: Deploy Your Textbook Now

## ⚡ 5-Minute Setup

### 1️⃣ Create GitHub Repo

Go to https://github.com/new and create:
- **Repository name**: `agentic-ai-textbook`
- **Description**: "Interactive textbook for RAGUIUC Agentic AI Club"
- **Do NOT check** "Initialize with README"

Copy the HTTPS URL (e.g., `https://github.com/RAGUIUC/agentic-ai-textbook.git`)

### 2️⃣ Push Code to GitHub

```bash
cd /Users/ash/Desktop/RAGUIUC

git init
git add .
git commit -m "Initial commit: Agentic AI Textbook"
git branch -M main
git remote add origin YOUR_REPO_URL_HERE
git push -u origin main
```

Replace `YOUR_REPO_URL_HERE` with your repository URL!

### 3️⃣ Enable GitHub Pages

1. Go to your repository
2. **Settings** → **Pages**
3. Under "Build and deployment":
   - Branch: **gh-pages**
   - Folder: **root**
4. Click **Save**

### 4️⃣ Wait for Deploy

1. Go to **Actions** tab
2. Watch "Deploy Jupyter Book to GitHub Pages" workflow
3. Wait for green checkmark ✅ (takes 2-3 minutes)

### 5️⃣ View Your Site

```
https://RAGUIUC.github.io/agentic-ai-textbook
```

Replace `RAGUIUC` with your GitHub username/org!

---

## 📁 Project Structure

```
agentic-ai-textbook/
├── _config.yml              # Book configuration
├── _toc.yml                 # Table of contents
├── intro.md                 # Landing page
├── Chapter_1_What_Are_AI_Agents.ipynb
├── requirements.txt         # Python dependencies
├── README.md                # Project description
├── CONTRIBUTING.md          # How to contribute
├── DEPLOYMENT.md            # Detailed deployment guide
├── copilot-instructions.md  # Agent guidelines
├── LICENSE                  # MIT license
├── .gitignore              # Git ignore rules
└── .github/
    └── workflows/
        └── deploy.yml       # Auto-deploy on push
```

---

## 🚀 Next Steps

### Add More Chapters

1. Create `Chapter_2_Agent_Planning.ipynb`
2. Edit `_toc.yml` to include it
3. Commit and push:
   ```bash
   git add Chapter_2_Agent_Planning.ipynb _toc.yml
   git commit -m "Add Chapter 2"
   git push
   ```
4. GitHub Actions automatically rebuilds! ✨

### Test Locally (Optional)

```bash
pip install jupyter-book
jupyter-book build .
open _build/html/index.html
```

---

## ✅ Deployment Checklist

- [ ] Created GitHub repository
- [ ] Pushed code to GitHub
- [ ] Enabled GitHub Pages in settings
- [ ] GitHub Actions workflow completed
- [ ] Site is live and accessible
- [ ] All notebooks render correctly

---

## 🆘 Troubleshooting

### Deploy failed?
- Check **Actions** tab for error details
- Most common: Missing Python dependency (add to `requirements.txt`)

### Site not showing up?
- Wait 1-2 minutes after workflow completes
- Hard refresh browser (Cmd+Shift+R)
- Check URL matches your repository name

### Need more help?
- See **DEPLOYMENT.md** for detailed guide
- Check [Jupyter Book docs](https://jupyterbook.org/)

---

## 📞 Support

Questions? Open an issue or ask in the RAGUIUC Discord!

**Congratulations!** 🎉 Your textbook is now live and will auto-update every time you push!
