# CLAUDE.md

This file provides guidance for AI assistants (Claude Code and others) working in this repository.

## Repository Overview

**jinming.github.io** is a personal GitHub Pages site for user Jinmaruko. It is currently a minimal skeleton with no framework, build system, or content established yet. This is a blank-slate repository ready for development.

- **Hosting**: GitHub Pages (`<username>.github.io` naming convention)
- **Current state**: Initial commit only — one `README.md` file
- **Framework**: None configured yet (open to Jekyll, Hugo, plain HTML, or other static site generators)

## Repository Structure

```
jinming.github.io/
├── README.md       # Repo description (one line)
└── CLAUDE.md       # This file
```

As content and structure are added, update this section to reflect the actual layout.

## Development Conventions

Since no framework has been chosen yet, follow these general conventions until a stack is established:

### Git Workflow
- **Main branch**: `master` — stable, deployed to GitHub Pages
- **Feature branches**: `<scope>/short-description` (e.g., `feature/add-blog`, `fix/header-layout`)
- Write clear, descriptive commit messages in the imperative mood (e.g., "Add blog post index page")
- Never force-push to `master`

### Adding a Static Site Framework
When a framework is chosen, document the setup here. Common choices for GitHub Pages:

| Framework | Config file | Build command | Output dir |
|-----------|-------------|---------------|------------|
| Jekyll    | `_config.yml` | `bundle exec jekyll build` | `_site/` |
| Hugo      | `hugo.toml` / `config.yml` | `hugo` | `public/` |
| Plain HTML | _(none)_ | _(none)_ | root or `docs/` |

### Content Conventions (to be established)
Once a framework is chosen:
- Document where blog posts live (e.g., `_posts/`, `content/blog/`)
- Document where static assets live (e.g., `assets/`, `static/`)
- Document the frontmatter format required for posts/pages

## Build & Deployment

- **Deployment**: Automatic via GitHub Pages on push to `master`
- **No CI/CD configured** — no GitHub Actions workflows exist yet
- **No build step required** until a framework is added

If a build step is added, create `.github/workflows/deploy.yml` and document the build command here.

## Key Notes for AI Assistants

1. **This repo is in its infancy.** Do not assume any framework, directory structure, or convention exists beyond what is documented here.
2. **Do not create files speculatively.** Only add files that are explicitly requested or clearly required by the task.
3. **Update this file** whenever a significant architectural decision is made (framework choice, content structure, CI/CD setup, styling approach).
4. **Branch targeting**: Development work should go on feature branches. Do not commit directly to `master` unless making trivial documentation changes.
5. **No package manager configured.** Do not run `npm install`, `bundle install`, or equivalent commands unless the relevant config file (`package.json`, `Gemfile`, etc.) has been added first.
6. **GitHub Pages constraints**: Only content in the repo root (or a `/docs` folder, or a `gh-pages` branch) is served. Respect this when choosing an output directory.
