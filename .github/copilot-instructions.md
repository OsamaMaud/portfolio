# AI Agent Instructions for Gradfolio Portfolio Site

This is a Jekyll-based portfolio website using the Gradfolio theme. Here's what you need to know to work effectively with this codebase:

## Project Architecture

- **Jekyll Structure**: Standard Jekyll site with custom collections for projects
- **Key Directories**:
  - `_layouts/`: Page templates (default.html, post.html, etc.)
  - `_includes/`: Reusable components and partials
  - `_projects/`: Collection for portfolio projects
  - `_posts/`: Blog posts in markdown format
  - `assets/css/_sass/`: SCSS styling components

## Content Patterns

1. **Project Pages**
   - Located in `_projects/` directory
   - Follow front matter pattern from existing projects
   - Order is controlled in `_config.yml` collections section

2. **Blog Posts**
   - Located in `_posts/` directory
   - File naming: `YYYY-MM-DD-title.md`
   - Required front matter: title, layout: post

## Theme Features

- **Dark Mode Support**: Built-in dark mode respects system preferences
- **Responsive Design**: Uses SCSS variables in `assets/css/_sass/variables.scss`
- **Social Integration**: Configure social links in `_config.yml`

## Development Workflow

1. **Local Development**:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```

2. **Configuration**:
   - Site settings in `_config.yml`
   - Navigation in `_includes/navigation.html`
   - Social footer in `_includes/social-footer.html`

3. **Content Guidelines**:
   - Use Kramdown markdown syntax
   - Images go in `assets/images/`
   - Custom styling in `assets/css/main.scss`

## Common Tasks

- **Adding a Project**: Create new .md file in `_projects/` and add to collection order in `_config.yml`
- **Customizing Style**: Modify variables in `assets/css/_sass/variables.scss`
- **Social Links**: Update in `_config.yml` under "Social media links in footer"

## Important Notes

- Don't modify `_layouts/compress.html` - it's for HTML optimization
- Keep image sizes optimized for web performance
- Use relative links with `{{ site.baseurl }}` prefix for internal links