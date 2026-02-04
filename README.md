# Johnattan Garcia Ruiz - Personal Website

Personal academic website for Johnattan Garcia Ruiz, MPH, MBA, LL.B., Department Associate at Harvard T.H. Chan School of Public Health.

## Tech Stack

- **Jekyll** - Static site generator
- **HTML/CSS** - Custom styling with CSS variables
- **GitHub Pages** - Hosting
- **Markdown** - Content creation

## Project Structure

```
j-garciaruiz.github.io/
├── _config.yml              # Jekyll configuration
├── _layouts/                # Layout templates
│   ├── default.html        # Base HTML structure
│   ├── home.html           # Homepage layout
│   ├── page.html           # Standard page layout
│   └── post.html           # Blog post layout
├── _includes/              # Reusable components
│   ├── navigation.html     # Site navigation
│   └── footer.html         # Site footer
├── _posts/                 # Blog posts (Jekyll format)
│   └── YYYY-MM-DD-title.md # Blog post files
├── index.md                # Homepage content
├── publications.html       # Publications page
├── visualizations.html     # Data visualizations gallery
├── blog.html               # Blog listing page (permalinked to /blog/)
├── style.css               # Main stylesheet
├── Gemfile                 # Ruby dependencies
└── sitemap.xml             # SEO sitemap
```

## Local Development Setup

### Prerequisites

- Ruby (version 2.7 or higher)
- RubyGems
- Bundler

### Installation

1. Clone the repository:
```bash
git clone https://github.com/j-garciaruiz/j-garciaruiz.github.io.git
cd j-garciaruiz.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Run the local development server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to:
```
http://localhost:4000
```

The site will automatically rebuild when you make changes to files.

## Creating Blog Posts

Blog posts are written in Markdown and stored in the `_posts/` directory.

### File Naming Convention

Posts must follow this naming pattern:
```
YYYY-MM-DD-title-with-dashes.md
```

Example: `2024-03-15-health-systems-reform.md`

### Blog Post Template

Create a new file in `_posts/` with the following front matter:

```markdown
---
layout: post
title: "Your Post Title Here"
date: 2024-03-15
category: "Health Systems"
tags:
  - Universal Coverage
  - Colombia
  - Health Policy
---

Your content goes here. You can use Markdown formatting.

## Subheadings

- Bullet points
- Lists
- **Bold text**
- *Italic text*

![Image alt text](path-to-image.jpg)

[Links](https://example.com)
```

### Publishing Posts

1. Create your post file in `_posts/`
2. Commit and push to the repository:
```bash
git add _posts/your-new-post.md
git commit -m "Add new blog post: Title"
git push origin main
```

3. GitHub Pages will automatically build and publish your changes

## Updating Content

### Homepage

Edit `index.md` - The file uses Jekyll front matter and HTML for structured content.

### Publications

Edit `publications.html` - Add new publications to the appropriate section.

### Visualizations

Edit `visualizations.html` - Add new visualization cards with embed codes.

### Site Configuration

Edit `_config.yml` to update:
- Site metadata
- Author information
- Social media links
- Navigation menu items

## GitHub Pages Configuration

This site is configured to work with GitHub Pages automatically. The following files are critical:

- `_config.yml` - Jekyll configuration
- `Gemfile` - Ruby dependencies
- `.gitignore` - Excludes build files from version control

### Deployment

Changes pushed to the `main` branch (or `master` depending on your repository settings) are automatically deployed to:
```
https://j-garciaruiz.github.io
```

## SEO Features

- Meta tags for social media (Open Graph, Twitter Cards)
- `jekyll-seo-tag` plugin for automated SEO
- `sitemap.xml` for search engines
- Descriptive page titles and descriptions

## Customization

### Colors

Edit CSS variables in `style.css`:

```css
:root {
    --color-primary: #1a365d;
    --color-secondary: #2c5282;
    --color-accent: #3182ce;
    /* ... other variables ... */
}
```

### Typography

The site uses Inter font from Google Fonts. To change:

1. Update the Google Fonts link in `_layouts/default.html`
2. Update the font-family in `style.css`

### Navigation

Edit the `navigation` array in `_config.yml`:

```yaml
navigation:
  - title: About
    url: /#about
  - title: New Page
    url: /new-page.html
```

## Responsive Design

The site is fully responsive with breakpoints at:
- 768px (tablets)
- 480px (mobile phones)

Test responsiveness by resizing your browser or using developer tools.

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Troubleshooting

### Jekyll Build Errors

If you encounter build errors:

```bash
bundle exec jekyll clean
bundle exec jekyll build --verbose
```

### Dependency Issues

Update dependencies:

```bash
bundle update
```

### Local Server Issues

If port 4000 is in use:

```bash
bundle exec jekyll serve --port 4001
```

## Future Enhancements

Potential improvements:
- Convert remaining pages (publications, visualizations, blog) to Jekyll layouts
- Add pagination for blog posts
- Implement search functionality
- Add comment system for blog posts
- Create automatic publication import from Google Scholar API

## License

© 2026 Johnattan Garcia Ruiz. All rights reserved.

## Contact

For website issues or questions:
- GitHub Issues: [https://github.com/j-garciaruiz/j-garciaruiz.github.io/issues](https://github.com/j-garciaruiz/j-garciaruiz.github.io/issues)
- Twitter: [@GarciaRuizJo](https://twitter.com/GarciaRuizJo)
