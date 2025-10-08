# Suchac.dev

Personal website and blog built with Jekyll and hosted on GitHub Pages.

🔗 **Live site**: [https://suchac.dev](https://suchac.dev)

## About

This is a personal portfolio and blog featuring:
- Personal bio and introduction
- Blog posts archive
- Projects showcase
- Responsive design with Bootstrap

## Getting Started

### Prerequisites

- Ruby (2.5 or higher)
- Jekyll
- Bundler

### Installation

```bash
bundle install
```

### Local Development

```bash
# Serve the site locally
bundle exec jekyll serve

# Site will be available at http://localhost:3000
```

### Building

```bash
# Build the site (output goes to _site/)
bundle exec jekyll build
```

## Project Structure

```
.
├── _config.yml           # Site configuration
├── _includes/            # Reusable components (header, footer, etc.)
├── _layouts/             # Page templates
├── _posts/               # Blog posts (Markdown files)
├── static/               # CSS, JS, and images
├── index.html            # Homepage
├── blog.html             # Blog archive
└── projects.html         # Projects page
```

## Creating Blog Posts

Add new posts to the `_posts/` directory with the format:

```
YYYY-MM-DD-post-title.md
```

Include front matter:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
tags: [tag1, tag2]
---

Your content here...
```

## Configuration

Edit `_config.yml` to customize:
- Site title and description
- Author information
- Social media links
- Base URL and permalink structure

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the `master` branch.

## License

Personal project - all rights reserved
