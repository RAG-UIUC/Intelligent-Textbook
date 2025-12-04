# How to Contribute

This intelligent textbook is a community project, and we welcome your contributions!

## Ways to Contribute

### 1. **Improve Existing Content**
- Fix typos or errors
- Clarify explanations
- Add better examples
- Improve code quality
- Suggest better visualizations

### 2. **Add New Chapters**
- Teach a new topic in agentic engineering
- Follow our [structure guide](https://github.com/RAG-UIUC/Intelligent-Textbook/blob/main/docs/STRUCTURE.md)
- Create an overview page and interactive notebook
- Include challenges and exercises

### 3. **Report Issues**
- Found a broken link?
- Code doesn't work?
- Concept unclear?
- Let us know!

### 4. **Share Feedback**
- What's working well?
- What could be better?
- What topics should we add?

## Getting Started

### Step 1: Fork the Repository
Go to [GitHub](https://github.com/RAG-UIUC/Intelligent-Textbook) and fork the repository.

### Step 2: Clone Your Fork
```bash
git clone https://github.com/YOUR-USERNAME/Intelligent-Textbook.git
cd Intelligent-Textbook
```

### Step 3: Create a Branch
```bash
git checkout -b feature/your-feature-name
```

### Step 4: Make Your Changes
- Edit or create files
- Test locally if possible
- Follow our content guidelines (below)

### Step 5: Commit & Push
```bash
git add .
git commit -m "Describe your changes clearly"
git push origin feature/your-feature-name
```

### Step 6: Open a Pull Request
Go to GitHub and create a pull request. Describe:
- What you changed and why
- Any relevant context
- If it fixes an issue, mention it

---

## Content Guidelines

### For Overview Pages (`index.md`)

Structure your overview with:

1. **Title & Description**
   - Clear, engaging title
   - What students will learn

2. **Core Concepts** (3-5)
   - Explain each concept clearly
   - Use examples and analogies
   - Include diagrams if helpful

3. **Sample Code**
   - Show key implementation
   - Keep it concise (10-20 lines)
   - Highlight the main pattern

4. **Links to Notebook**
   - "Explore this interactively →"
   - Make it obvious what's next

5. **Resources**
   - Links to further reading
   - References and citations

### For Interactive Notebooks

Structure your notebook with:

1. **Introduction**
   - What this notebook covers
   - How to use it
   - Prerequisites

2. **Detailed Explanations**
   - Deep dive into concepts
   - Real-world context
   - Why it matters

3. **Code Examples**
   - Runnable, well-commented code
   - Multiple examples per concept
   - Error handling

4. **Interactive Widgets**
   - Let users experiment
   - Adjust parameters and see results
   - Real-time feedback

5. **Visualizations**
   - Plots and diagrams
   - Animations when helpful
   - Making concepts visual

6. **Key Takeaways**
   - Summary of main ideas
   - What to remember

7. **Challenge Exercises**
   - 2-3 problems to solve
   - Solutions provided (hidden)
   - Increasing difficulty

### Code Style

- Use **clear variable names**
- Add **comments explaining logic**
- Follow **PEP 8** conventions
- Include **docstrings** for functions
- Keep **examples runnable** with no external dependencies

```python
def meaningful_function_name(parameter):
    """
    Clear explanation of what this does.
    
    Args:
        parameter: What this parameter represents
    
    Returns:
        What the function returns
    """
    # Implementation with clear comments
    result = do_something(parameter)
    return result
```

### Writing Style

- **Clear & Concise** - Get to the point
- **Engaging** - Show why this matters
- **Progressive** - Build from simple to complex
- **Accessible** - Avoid jargon or explain it
- **Practical** - Include real examples

---

## Adding a New Chapter

### 1. Create Folder Structure
```
chapters/NN-chapter-name/
├── index.md           (overview)
└── notebook.ipynb     (interactive)
```

Use zero-padded numbers (01, 02, 03) and kebab-case names.

### 2. Write Overview (`index.md`)

Follow the content guidelines above. Make it:
- Standalone - explains concepts clearly
- Engaging - uses examples and analogies
- Visual - includes diagrams if helpful
- Linked - clearly links to the notebook

### 3. Create Notebook (`notebook.ipynb`)

Follow the notebook guidelines above. Make it:
- Runnable - all code works without errors
- Interactive - includes widgets and controls
- Visual - has plots and visualizations
- Comprehensive - covers the topic thoroughly

### 4. Update Table of Contents

Edit `_toc.yml`:
```yaml
- file: chapters/NN-chapter-name/index.md
  title: Chapter N - Chapter Title
  sections:
    - file: chapters/NN-chapter-name/notebook.ipynb
      title: "Interactive Notebook: Deep Dive"
```

### 5. Test Your Changes

Build locally:
```bash
pip install jupyter-book
jupyter-book build .
open _build/html/index.html
```

Verify:
- ✅ Navigation works
- ✅ Links are correct
- ✅ Code runs without errors
- ✅ Formatting looks good

### 6. Submit Pull Request

Push your changes and create a pull request!

---

## Review Process

When you submit a pull request, we'll:

1. **Check Quality** - Does it follow guidelines?
2. **Test Content** - Do code examples work?
3. **Verify Structure** - Is the navigation correct?
4. **Provide Feedback** - Suggestions for improvement?
5. **Merge** - Your contribution goes live!

This usually takes a few days. We may ask for revisions.

---

## Helpful Resources

- [Markdown Guide](https://www.markdownguide.org/) - Formatting guide
- [Jupyter Notebook Docs](https://jupyter-notebook.readthedocs.io/) - Creating notebooks
- [GitHub Help](https://docs.github.com/en) - How to use GitHub
- [Our Structure Guide](https://github.com/RAG-UIUC/Intelligent-Textbook/blob/main/docs/STRUCTURE.md) - Folder organization

---

## Questions?

- **Setup Issues?** Check existing issues or ask in discussions
- **Content Questions?** Review our guidelines above
- **Technical Help?** Check GitHub documentation

---

## Code of Conduct

We're committed to providing a welcoming environment. Please be respectful and constructive in all interactions.

---

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (CC BY-NC-SA 4.0).

---

**Thank you for contributing to make agentic engineering accessible to everyone!** 🎓

Your work matters and will help students and researchers worldwide understand and build intelligent systems.
