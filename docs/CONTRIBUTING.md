# Contributing to the Agentic AI Textbook

Thank you for interest in contributing! This guide will help you add content to our textbook.

## 🎯 What We Need

- **New Chapters**: Follow the Chapter 1 template
- **Improvements**: Better explanations, clearer examples
- **Exercises**: Challenge problems for students
- **Bug Fixes**: Corrections in existing content
- **Documentation**: Better guides and tutorials

## 📝 Writing a Chapter

### Template Structure

Each chapter should include:

```markdown
# Chapter N: [Topic Name]

## [Section 1]

[Explanation in markdown]

## Interactive Element / Code Example

[Python code cells with explanations]

## [Section 2]

[More content]

## 🎓 Key Takeaways

- Point 1
- Point 2
- Point 3

## 💡 Challenge Exercise

[Problem for students to solve]
```

### Best Practices

1. **Use Clear Headings**: Organize content with markdown headers
2. **Mix Text and Code**: Alternate explanations with executable cells
3. **Add Visuals**: Use plots, diagrams, and animations
4. **Interactive Widgets**: Use ipywidgets for user input
5. **Real Examples**: Ground concepts in practical applications
6. **Challenge Exercises**: End each chapter with problems
7. **Keep It Concise**: Explain clearly without unnecessary length

## 🚀 Submission Process

### 1. Fork and Clone

```bash
git clone https://github.com/YOUR_USERNAME/agentic-ai-textbook.git
cd agentic-ai-textbook
git checkout -b feature/chapter-name
```

### 2. Create Your Chapter

Create a new Jupyter notebook:
```bash
jupyter notebook Chapter_N_Topic_Name.ipynb
```

Write your content following the template above.

### 3. Update Table of Contents

Edit `_toc.yml` to add your chapter:
```yaml
- file: Chapter_N_Topic_Name.ipynb
  title: Chapter N - Topic Name
  sections:
    - file: subsection.ipynb
      title: "Subsection Title"
```

### 4. Test Locally

```bash
# Install dependencies
pip install -r requirements.txt
pip install jupyter-book

# Build and preview
jupyter-book build .
open _build/html/index.html
```

### 5. Commit and Push

```bash
git add Chapter_N_Topic_Name.ipynb _toc.yml
git commit -m "Add Chapter N: Topic Name"
git push origin feature/chapter-name
```

### 6. Create Pull Request

Go to GitHub and create a pull request. Describe:
- What your chapter covers
- Who it's for (all students, advanced, etc.)
- Any prerequisites
- Learning objectives

## 📋 Code Style Guide

### Python Code

```python
# Use clear variable names
# Add comments for complex logic
# Follow PEP 8 conventions

def my_function(parameter1, parameter2):
    """
    Clear docstring explaining what this does.
    
    Args:
        parameter1: What this parameter is
        parameter2: What this parameter is
    
    Returns:
        What this function returns
    """
    result = parameter1 + parameter2
    return result
```

### Markdown

```markdown
# Main Title (H1)

Use **bold** and *italic* sparingly.

## Section Heading (H2)

### Subsection (H3)

- Use bullet points
- For lists of items
- Keep them concise

> Use blockquotes for important notes

`code_in_backticks` for inline code
```

## 🎨 Visualization Guide

### Matplotlib (Static Plots)

```python
import matplotlib.pyplot as plt

fig, ax = plt.subplots(figsize=(10, 6))
ax.plot(x, y, label='Line')
ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.legend()
plt.show()
```

### Plotly (Interactive Plots)

```python
import plotly.express as px

fig = px.scatter(data, x='x_col', y='y_col', title='Title')
fig.show()
```

### Interactive Widgets

```python
from ipywidgets import IntSlider, interactive

def my_function(x):
    return x ** 2

interactive(my_function, x=IntSlider(min=0, max=10))
```

## 📚 Chapter Topic Ideas

- **Chapter 2**: Agent Planning & Reasoning
- **Chapter 3**: Tool Integration & Function Calling
- **Chapter 4**: Multi-Agent Systems
- **Chapter 5**: Learning & Adaptation
- **Chapter 6**: Real-World Applications
- **Chapter 7**: Advanced Architectures
- **Chapter 8**: Evaluating Agent Performance

## ❓ Questions?

- Check existing chapters for examples
- Ask in pull request comments
- Open an issue with questions
- Reach out in the RAGUIUC Discord

## ✅ Review Checklist

Before submitting, ensure:

- [ ] Chapter follows template structure
- [ ] Code runs without errors locally
- [ ] All cells produce output
- [ ] Explanations are clear and concise
- [ ] Interactive elements work
- [ ] Links are correct
- [ ] Images load properly
- [ ] References are cited if applicable
- [ ] Challenge exercise is included
- [ ] `_toc.yml` is updated

## 🎉 Thank You!

Your contributions make this textbook better for everyone. We can't wait to see what you create!

---

**Happy Contributing!** 🚀
