# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal website and blog hosted on GitHub Pages at https://suchac.dev. The site features:
- Personal homepage with bio and social links
- Blog archive page
- Projects showcase page
- Bootstrap-based responsive design

## Development Commands

### Local Development
```bash
# Install dependencies (if not already installed)
bundle install

# Serve the site locally (configured to run on port 3000)
bundle exec jekyll serve
# Site will be available at http://localhost:3000
```

### Build
```bash
# Build the site (output goes to _site/ directory)
bundle exec jekyll build
```

## Architecture

### Jekyll Structure
- `_config.yml` - Main site configuration (title, author, social links, baseurl, pagination)
- `_layouts/` - HTML templates that wrap content
  - `layout.html` - Base template with header, footer, Bootstrap, and GitHub corner ribbon
  - `home.html` - Simple wrapper that extends layout.html
  - `page.html` - Generic page template
  - `post.html` - Blog post template with date, tags, and related posts
- `_includes/` - Reusable HTML components (header, footer, social, projects, analytics, disqus)
- `_posts/` - Blog posts in Markdown (currently empty)
- `static/` - Static assets (CSS, JS, images)
  - `css/` - Bootstrap overrides and custom styles
  - `js/` - Bootstrap and custom JavaScript
  - `img/` - Images and favicons

### Key Pages
- `index.html` - Homepage using home layout, displays personal bio
- `blog.html` - Blog archive listing all posts by date
- `projects.html` - Projects showcase page
- `404.html` - Custom 404 error page

### Site Configuration
The site is configured in `_config.yml` with:
- URL: https://suchac.dev
- Port 3000 for local development
- Kramdown markdown processor with Rouge syntax highlighting
- Pagination set to 5 posts per page
- Permalink format: `/:title.html`

### Content Management
- Blog posts should be created in `_posts/` directory with format: `YYYY-MM-DD-post-title.md`
- Posts must include front matter with layout, title, date, and optional tags
- Projects are managed through `_includes/projects.html`
- Site metadata (author name, social links, description) configured in `_config.yml`

### Build Output
- Generated site files go to `_site/` (gitignored)
- Jekyll metadata cached in `.jekyll-metadata` (gitignored)
