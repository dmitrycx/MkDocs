# MkDocs + Material Test Project

A test project for exploring [MkDocs](https://www.mkdocs.org/) with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

## Prerequisites

- Python 3.8+
- pip

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/dmitrycx/MkDocs.git
cd MkDocs
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the development server

```bash
mkdocs serve
```

### 5. Open in browser

Navigate to http://127.0.0.1:8000

The site will auto-reload when you edit any markdown files in `docs/`.

## Project Structure

```
.
├── docs/                       # Documentation source files
│   ├── index.md               # Homepage
│   ├── assets/                # Logo, images, custom CSS
│   ├── concepts/              # Core concepts (Requests, etc.)
│   ├── features/              # Feature documentation
│   ├── how-to/                # Step-by-step guides
│   └── faq/                   # Frequently asked questions
├── mkdocs.yml                 # MkDocs configuration
└── requirements.txt           # Python dependencies
```

## Useful Commands

| Command | Description |
|---------|-------------|
| `mkdocs serve` | Start dev server with live reload |
| `mkdocs build` | Build static site to `site/` |
| `mkdocs gh-deploy` | Deploy to GitHub Pages |

## Resources

- [MkDocs Documentation](https://www.mkdocs.org/)
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [Material Reference](https://squidfunk.github.io/mkdocs-material/reference/)
