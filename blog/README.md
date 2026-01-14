# My Quarto Blog

A technical blog built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

**Live Site**: https://junliliu1.github.io/My-Quarto-Blog-for-542

## 📝 About

This blog is created for sharing data science and programming learning notes, projects, and technical insights.

## 🚀 Quick Start

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) installed
- Git
- GitHub account

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/junliliu1/My-Quarto-Blog-for-542.git
cd My-Quarto-Blog-for-542
```

2. Preview the blog locally:
```bash
quarto preview
```

3. The blog will open at `http://localhost:4200` (or another port)

## ✍️ Creating New Posts

### Method 1: Manual Creation

1. Create a new directory in `posts/`:
```bash
mkdir posts/my-new-post
cd posts/my-new-post
```

2. Create `index.qmd` with the following template:
```yaml
---
title: "Your Post Title"
author: "Your Name"
date: "2026-01-14"
categories: [data-science, python, tutorial]
image: "thumbnail.jpg"  # Optional
draft: false
---

## Introduction

Your content here...

### Code Example

```python
import pandas as pd
print("Hello, Quarto!")
```
```

3. Add images/assets to the same directory

### Method 2: Using Template

You can duplicate one of the existing posts in the `posts/` directory and modify it.

## 🏗️ Project Structure

```
.
├── .github/
│   └── workflows/
│       └── publish.yml      # GitHub Actions workflow
├── posts/                   # All blog posts
│   ├── _metadata.yml        # Shared post metadata
│   ├── welcome/
│   └── post-with-code/
├── _quarto.yml              # Main configuration
├── index.qmd                # Blog homepage
├── about.qmd                # About page
├── styles.css               # Custom styles
├── .gitignore
├── .nojekyll                # For GitHub Pages
└── README.md
```

## 🎨 Customization

### Change Theme

Edit `_quarto.yml`:
```yaml
format:
  html:
    theme: [cosmo, darkly, flatly, journal, ...]
```

Available themes: cosmo, darkly, flatly, journal, litera, lumen, lux, materia, minty, morph, pulse, quartz, sandstone, simplex, sketchy, slate, solar, spacelab, superhero, united, vapor, yeti, zephyr

### Update Personal Info

Edit `about.qmd` to add your bio, profile picture, and social links.

### Modify Navigation

Edit `_quarto.yml` under `website.navbar` section.

## 📤 Publishing

### Automatic Deployment (Recommended)

The blog is configured with GitHub Actions for automatic deployment:

1. Push changes to the `main` or `master` branch
2. GitHub Actions will automatically build and deploy

### Manual Deployment

```bash
quarto publish gh-pages
```

## ⚙️ GitHub Pages Setup

If this is your first time setting up:

1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under "Build and deployment":
   - **Source**: GitHub Actions
4. Wait for the GitHub Action to complete
5. Your site will be live at: https://junliliu1.github.io/My-Quarto-Blog-for-542

## 📚 Useful Resources

- [Quarto Documentation](https://quarto.org/docs/guide/)
- [Quarto Blog Guide](https://quarto.org/docs/websites/website-blog.html)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Quarto Publishing Guide](https://quarto.org/docs/publishing/github-pages.html)

## 🔧 Troubleshooting

### Preview not working
```bash
quarto check
```

### Build fails on GitHub Actions
- Check the Actions tab in your repository for error logs
- Ensure all required files are committed
- Verify `_quarto.yml` syntax

### 404 Error on GitHub Pages
- Ensure `.nojekyll` file exists in the root
- Check that GitHub Pages is configured correctly in repository settings
- Wait a few minutes for deployment to complete

## 📄 License

This blog content is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## 👤 Author

**Jun Li Liu**

- GitHub: [@junliliu1](https://github.com/junliliu1)
- Blog: https://junliliu1.github.io/My-Quarto-Blog-for-542
