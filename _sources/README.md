# Agentic Engineering Textbook

Interactive textbook for the **RAGUIUC Agentic AI Club** teaching agentic engineering principles through hands-on Jupyter notebooks.

## 📖 View the Textbook

Visit the deployed textbook: **[https://rag-uiuc.github.io/Intelligent-Textbook/](https://rag-uiuc.github.io/Intelligent-Textbook/)**

---

## 📁 Project Structure

```
Intelligent-Textbook/
├── chapters/                          # All chapter content
│   └── 01-what-are-agents/           # Chapter 1 folder
│       ├── index.md                  # Chapter overview & concepts
│       └── notebook.ipynb            # Interactive notebook
│
├── docs/                              # Documentation
│   ├── README.md                     # Full project documentation
│   ├── CONTRIBUTING.md               # How to contribute chapters
│   ├── DEPLOYMENT.md                 # Deployment guide
│   └── QUICKSTART.md                 # Quick setup guide
│
├── assets/                            # Images, logos, resources
│   └── (placeholder for future assets)
│
├── intro.md                           # Landing page
├── _config.yml                        # Jupyter Book configuration
├── _toc.yml                          # Table of contents
├── requirements.txt                   # Python dependencies
├── LICENSE                           # MIT license
├── copilot-instructions.md           # AI agent guidelines
└── .github/
    └── workflows/
        └── deploy.yml                # Auto-deployment workflow
```

---

## 🚀 Features

- **Interactive Notebooks**: Run code cells directly in the browser
- **Organized Chapters**: Each chapter in its own folder with overview + notebook
- **Visualizations**: Dynamic plots and real-time simulations
- **Challenge Exercises**: Hands-on problems to deepen learning
- **Responsive Design**: Works on desktop and mobile
- **Full-Text Search**: Easily find topics across chapters

---

## 📚 Chapters

### Chapter 1: What Are AI Agents?
- **Overview**: Concepts and foundational theory
- **Notebook**: Interactive code examples and experiments

More chapters coming soon!

---

## 🛠️ Quick Start

### View Online
Simply visit: **[https://rag-uiuc.github.io/Intelligent-Textbook/](https://rag-uiuc.github.io/Intelligent-Textbook/)**

### Build Locally

```bash
# Clone repository
git clone https://github.com/RAG-UIUC/Intelligent-Textbook.git
cd Intelligent-Textbook

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
pip install jupyter-book

# Build the book
jupyter-book build .

# View locally
open _build/html/index.html  # macOS
# or open in Windows/Linux
```

---

## 📝 Contributing

Want to add a new chapter? Follow these steps:

### 1. Create Chapter Folder
```bash
mkdir chapters/02-agent-planning
touch chapters/02-agent-planning/index.md
touch chapters/02-agent-planning/notebook.ipynb
```

### 2. Write Overview
Create `index.md` with:
- Concepts and explanations
- Links to the notebook
- Learning objectives
- Resources

### 3. Create Interactive Notebook
Create `notebook.ipynb` with:
- Detailed implementations
- Interactive widgets
- Real-time visualizations
- Challenge exercises

### 4. Update Table of Contents
Edit `_toc.yml`:
```yaml
- file: chapters/02-agent-planning/index.md
  title: Chapter 2 - Agent Planning
  sections:
    - file: chapters/02-agent-planning/notebook.ipynb
      title: "Interactive Notebook"
```

### 5. Commit and Push
```bash
git add chapters/ _toc.yml
git commit -m "Add Chapter 2: Agent Planning"
git push
```

GitHub Actions will automatically build and deploy! ✨

See [docs/CONTRIBUTING.md](docs/CONTRIBUTING.md) for detailed guidelines.

---

## 🎓 Learning Path

This textbook follows a structured progression:

1. **Fundamentals** (Chapter 1)
   - What are agents?
   - Types of agents
   - Architecture and components

2. **Planning** (Chapter 2, coming soon)
   - How agents think ahead
   - Goal representation
   - Search algorithms

3. **Tools & Integration** (Chapter 3, coming soon)
   - Function calling
   - Tool integration
   - External knowledge

4. **Multi-Agent Systems** (Chapter 4, coming soon)
   - Multiple agents working together
   - Communication & coordination
   - Emergent behavior

5. **Advanced Topics** (Chapter 5+, coming soon)
   - Learning and adaptation
   - Real-world applications
   - Evaluation and deployment

---

## 💻 Technology Stack

- **Jupyter Book**: Static site generation from Jupyter notebooks
- **Python**: Code examples and interactive elements
- **GitHub Pages**: Hosting and deployment
- **GitHub Actions**: Automatic build and deployment

---

## 📖 Documentation Files

- **[docs/QUICKSTART.md](docs/QUICKSTART.md)** - Get started in 5 minutes
- **[docs/DEPLOYMENT.md](docs/DEPLOYMENT.md)** - Detailed deployment guide
- **[docs/CONTRIBUTING.md](docs/CONTRIBUTING.md)** - How to contribute
- **[docs/README.md](docs/README.md)** - Full project documentation

---

## 🎯 Best Practices

### For Students
- Start with chapter overviews to understand concepts
- Then run the notebook to see implementations
- Modify code to experiment and learn
- Complete challenges to test understanding

### For Contributors
- Each chapter = one folder with overview + notebook
- Overview: High-level concepts, links to notebook
- Notebook: Deep dives, code, widgets, challenges
- Keep code runnable and well-documented
- Include learning objectives and prerequisites

---

## 🆘 Troubleshooting

### Site not loading?
- Clear browser cache (Cmd+Shift+R on Mac)
- Wait 1-2 minutes for GitHub Pages to update
- Check Actions tab for build errors

### Notebook has errors?
- Run locally first: `jupyter notebook chapters/01-what-are-agents/notebook.ipynb`
- Check Python version (requires 3.9+)
- Ensure all dependencies in `requirements.txt`

### Can't find a topic?
- Use the search function (top right of site)
- Check table of contents in sidebar
- Visit chapter overview pages for links

---

## 📞 Support

- **Questions?** Open an issue on GitHub
- **Suggestions?** Create a discussion
- **Bugs?** Report with error details
- **Discord?** Join RAGUIUC for real-time help

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file

---

## 🎉 Credits

Built with ❤️ by **RAGUIUC Agentic AI Club**

*Making agentic engineering accessible and interactive for everyone.*

---

## 🗂️ File Organization

| Folder | Purpose |
|--------|---------|
| `chapters/` | All chapter content (overviews + notebooks) |
| `docs/` | Documentation & guides |
| `assets/` | Images, logos, resources |
| `.github/workflows/` | GitHub Actions automation |

**Chapter Structure**: Each chapter is self-contained with:
- `index.md` = Overview with concepts and sample code
- `notebook.ipynb` = Full interactive exploration

This makes it easy to find, add, and scale chapters! ✨
