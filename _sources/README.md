# Agentic Engineering Textbook

Interactive textbook for the **RAGUIUC Agentic AI Club** teaching agentic engineering principles through hands-on Jupyter notebooks.

## 📖 View the Textbook

Visit the deployed textbook: [https://agentic-ai-textbook.github.io/](https://agentic-ai-textbook.github.io/)

## 🚀 Features

- **Interactive Notebooks**: Run code cells directly in the browser
- **Visualizations**: Dynamic plots and real-time simulations
- **Challenge Exercises**: Hands-on problems to deepen learning
- **Responsive Design**: Works on desktop and mobile
- **Full-Text Search**: Easily find topics across chapters

## 📚 Chapters

1. **Chapter 1: What Are AI Agents?**
   - Agent fundamentals and the perception-action loop
   - Types of agents (reactive, deliberative, hybrid)
   - Building your first simple agent
   - Interactive simulations

More chapters coming soon!

## 🛠️ Building Locally

### Prerequisites
- Python 3.9+
- Git

### Setup

```bash
# Clone the repository
git clone https://github.com/RAGUIUC/agentic-ai-textbook.git
cd agentic-ai-textbook

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install jupyter-book
pip install jupyter-book

# Build the book
jupyter-book build .

# View locally
# Open _build/html/index.html in your browser
```

## 📝 Contributing

We welcome contributions! To add content:

1. Create a new branch: `git checkout -b feature/chapter-2`
2. Add your notebook or markdown file
3. Update `_toc.yml` to include your content
4. Test locally with `jupyter-book build .`
5. Create a pull request

## 🎓 For Club Members

- **Creating Chapters**: Use Jupyter notebooks (.ipynb format)
- **Adding Content**: Mix markdown text with executable Python code
- **Interactive Elements**: Use ipywidgets for sliders, buttons, and dropdowns
- **Visualizations**: Use matplotlib, plotly, or seaborn
- **Structure**: Each chapter should have clear sections and learning objectives

## 📋 Setup Checklist

- [ ] Clone this repository
- [ ] Create a GitHub repository at `https://github.com/RAGUIUC/agentic-ai-textbook`
- [ ] Push this code to your main branch
- [ ] Enable GitHub Pages in repository settings (source: gh-pages branch)
- [ ] Update `_config.yml` with your repository URL
- [ ] Verify the GitHub Actions workflow runs successfully
- [ ] Visit your site at `https://RAGUIUC.github.io/agentic-ai-textbook`

## ⚙️ Configuration

Key files:
- `_config.yml`: Jupyter Book configuration (title, theme, features)
- `_toc.yml`: Table of contents and chapter structure
- `intro.md`: Landing page content
- `.github/workflows/deploy.yml`: Automated deployment workflow

## 🤔 FAQ

**Q: How do I add a new chapter?**
A: Create a new `.ipynb` notebook, add it to `_toc.yml`, commit and push. GitHub Actions will automatically rebuild and deploy.

**Q: Can I use different Python versions?**
A: Yes, edit `.github/workflows/deploy.yml` and change the `python-version` value.

**Q: How do I fix build errors?**
A: Check the GitHub Actions log for details. Common issues: missing dependencies (add to `requirements.txt`), notebook errors (test locally first).

**Q: Can readers run code in the browser?**
A: Yes! Use the Binder integration (automatically available) - click the 🚀 icon on any page.

## 📞 Support

- **Issues**: Open an issue on GitHub
- **Questions**: Ask in the RAGUIUC Discord
- **Suggestions**: We'd love to hear your ideas!

## 📄 License

This project is licensed under the MIT License - see LICENSE file for details.

---

**Built with ❤️ by RAGUIUC Agentic AI Club**

*Making agentic engineering accessible and interactive for everyone.*
