# Deployment Guide

## Step-by-Step Deployment to GitHub Pages

### 1. Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Create a new repository named `agentic-ai-textbook`
3. **Do NOT initialize with README** (we have one already)
4. Copy the repository URL (e.g., `https://github.com/RAGUIUC/agentic-ai-textbook.git`)

### 2. Initialize Git and Push

```bash
cd /Users/ash/Desktop/RAGUIUC

# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Agentic AI Textbook with Chapter 1"

# Add remote repository
git remote add origin https://github.com/RAGUIUC/agentic-ai-textbook.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Build and deployment":
   - Select **Deploy from a branch**
   - Choose **gh-pages** as the branch
   - Select **root** as the folder
4. Wait for the page to refresh

### 4. GitHub Actions Workflow

The `.github/workflows/deploy.yml` file will automatically:
1. Run when you push to the `main` branch
2. Build the Jupyter Book
3. Deploy to the `gh-pages` branch
4. Update your live site

**Check the status:**
- Go to **Actions** tab in your repository
- Watch the "Deploy Jupyter Book to GitHub Pages" workflow run
- Once it completes (green checkmark), your site is live!

### 5. Access Your Site

Your textbook will be available at:
```
https://RAGUIUC.github.io/agentic-ai-textbook
```

(Replace `RAGUIUC` with your actual GitHub username/organization)

## 📝 Adding New Chapters

### To add Chapter 2:

1. Create a new Jupyter notebook: `Chapter_2_Agent_Planning.ipynb`
2. Edit `_toc.yml`:
   ```yaml
   - file: Chapter_2_Agent_Planning.ipynb
     title: Chapter 2 - Agent Planning & Reasoning
   ```
3. Commit and push:
   ```bash
   git add Chapter_2_Agent_Planning.ipynb _toc.yml
   git commit -m "Add Chapter 2: Agent Planning & Reasoning"
   git push
   ```
4. GitHub Actions automatically rebuilds and deploys!

## 🔧 Troubleshooting

### "Deploy failed" in GitHub Actions

**Check the workflow log:**
1. Go to Actions tab
2. Click the failed workflow
3. Expand "Build the book" step
4. Look for error messages

**Common fixes:**
- Missing dependency: Add to `requirements.txt`
- Notebook error: Test locally with `jupyter-book build .`
- Syntax error in YAML files: Validate `_config.yml` and `_toc.yml`

### "Page not found" after deployment

- Wait 1-2 minutes after the workflow completes
- Hard refresh your browser (Cmd+Shift+R on Mac)
- Verify the URL matches your repository name

### Local build errors

```bash
# Clear and rebuild
rm -rf _build/
jupyter-book build .
```

## 🎨 Customization

### Change the Title and Logo

Edit `_config.yml`:
```yaml
title: Your New Title
logo: path/to/logo.png
```

### Change the Theme

Edit `_config.yml`:
```yaml
html:
  theme: dark  # Options: light, dark
```

### Add More Features

See [Jupyter Book documentation](https://jupyterbook.org/) for:
- Custom CSS styling
- Citation management
- Interactive elements
- Advanced configurations

## 📦 Building Locally

To preview changes before pushing:

```bash
# Install dependencies (one time)
pip install -r requirements.txt
pip install jupyter-book

# Build the book
jupyter-book build .

# Open in browser
open _build/html/index.html
```

## ✅ Deployment Checklist

- [ ] GitHub repository created
- [ ] Repository initialized with `git init`
- [ ] All files committed and pushed to `main`
- [ ] GitHub Actions workflow triggered successfully
- [ ] GitHub Pages enabled in repository settings
- [ ] Workflow completed with green checkmark
- [ ] Site accessible at `https://username.github.io/agentic-ai-textbook`
- [ ] All notebooks render correctly
- [ ] Links and navigation working
- [ ] Mobile view looks good

## 🆘 Need Help?

1. Check [Jupyter Book docs](https://jupyterbook.org/)
2. Review [GitHub Pages help](https://docs.github.com/en/pages)
3. Check GitHub Actions logs for specific errors
4. Open an issue in the repository

Good luck with your deployment! 🚀
