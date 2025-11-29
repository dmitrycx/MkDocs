# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MkDocs documentation project using Material for MkDocs theme with modern features enabled.

## Commands

```bash
# Install dependencies
pip install -r requirements.txt

# Development server with live reload
mkdocs serve

# Build static site to site/
mkdocs build

# Deploy to GitHub Pages
mkdocs gh-deploy
```

## Project Structure

- `mkdocs.yml` - Main configuration (theme, plugins, extensions, navigation)
- `docs/` - Markdown source files
  - `concepts/` - Core concepts
  - `features/` - Feature documentation
  - `how-to/` - Step-by-step guides
  - `faq/` - FAQs
  - `assets/` - Logo, images, custom CSS
- `site/` - Generated output (gitignored)

## Key Configuration Features

The `mkdocs.yml` includes:
- **Theme**: Material with light/dark mode toggle
- **Navigation**: Instant loading, tabs, sections, scroll tracking
- **Code**: Syntax highlighting, copy buttons, annotations, Mermaid diagrams
- **Markdown**: Admonitions, content tabs, task lists, footnotes, tables

## Writing Documentation

Use these Material for MkDocs features in markdown files:
- Admonitions: `!!! note`, `!!! warning`, `!!! tip`, `!!! example`
- Code blocks with titles: ` ```python title="file.py" `
- Content tabs: `=== "Tab 1"`
- Mermaid diagrams in fenced code blocks
- Task lists: `- [x] Done` / `- [ ] Todo`

## Images

Store images in `docs/assets/images/` organized by topic:
```
docs/assets/images/requests/screenshot.png
```

Reference in markdown:
```markdown
![Alt text](../../assets/images/requests/screenshot.png)
```

## Customization

- **Logo**: `docs/assets/logo.svg`
- **Custom CSS**: `docs/assets/stylesheets/extra.css`
