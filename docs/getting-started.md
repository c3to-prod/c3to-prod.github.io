# Getting Started

This guide will help you get started with the documentation.

## Installation

To work with this documentation locally, you'll need to install MkDocs and its dependencies:

```bash
pip install -r requirements.txt
```

## Running Locally

To preview the documentation locally:

```bash
mkdocs serve
```

This will start a development server at `http://127.0.0.1:8000/`.

## Building the Site

To build the static site:

```bash
mkdocs build
```

The built site will be in the `site/` directory.

## Deployment

To deploy to GitHub Pages:

```bash
mkdocs gh-deploy
```

This will build the site and push it to the `gh-pages` branch.

## Adding New Pages

1. Create a new Markdown file in the `docs/` directory
2. Add it to the navigation in `mkdocs.yml`:

```yaml
nav:
  - Home: index.md
  - Your New Page: your-page.md
```

## Writing Documentation

### Headers

Use `#` for headers. The number of `#` symbols indicates the header level.

### Lists

- Bullet point 1
- Bullet point 2
  - Nested item

1. Numbered item 1
2. Numbered item 2

### Code Blocks

Use triple backticks with a language identifier:

```python
def example():
    return "Hello"
```

### Links

[Link text](https://example.com)

### Images

![Alt text](path/to/image.png)

## Tips

!!! tip "Tip"
    Save your files and the preview will auto-reload!

!!! warning "Warning"
    Don't commit the `site/` directory to git - it's built automatically.
