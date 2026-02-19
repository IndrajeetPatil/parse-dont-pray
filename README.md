# Parse, Don't Pray: The Case for Data Validation

This presentation explores the benefits of using data validation libraries like Pydantic (Python) and Zod (TypeScript) to create robust, maintainable applications.

The slides can be seen here:<br>
<https://indrajeetpatil.github.io/parse-dont-pray/>

<a href="https://indrajeetpatil.github.io/parse-dont-pray/" target="_blank">
<img src="media/social-media-card.jpg" alt="introductory slide" width="400"/>
</a>

# Development

This project uses Python 3.13+ with [uv](https://docs.astral.sh/uv/) for dependency management, [Quarto](https://quarto.org/) for rendering slides, and [just](https://github.com/casey/just) as a command runner.

## Prerequisites

```bash
# Install just (macOS)
brew install just
```

## Setup

```bash
# Install dependencies
just install

# Or update to latest versions
just update
```

## Common Commands

```bash
just help      # Show all available commands
just render    # Render slides to HTML
just preview   # Live preview with auto-reload
just open      # Open rendered slides in browser
just clean     # Remove generated files
just check     # Check Quarto and Python setup
just           # Install, render, and open slides (default)
```

## GitHub Pages deployment (automatic)

This repository uses GitHub Actions to render the slides and deploy the rendered `_site/` directory to GitHub Pages.

# Feedback

I'd love to hear thoughts and comments [here](https://github.com/IndrajeetPatil/parse-dont-pray/issues).

# Code of Conduct

Please note that the parse-dont-pray project is released with a [Contributor Code of Conduct](https://www.contributor-covenant.org/version/3/0/code_of_conduct/). By contributing to this project, you agree to abide by its terms.
