# Paw Pantry Mission Website

Official website for Paw Pantry Mission, a SEC-registered animal welfare organization in Cebu, Philippines.

## Quick Start

```bash
# Install dependencies
bundle install

# Start local development server
bundle exec jekyll serve

# Open in browser
open http://127.0.0.1:4000
```

## Prerequisites

- **Ruby** 2.7+ (check with `ruby --version`)
- **Bundler** (install with `gem install bundler`)
- **Git** (for version control)

## Development Commands

### Local Development

```bash
# Start server (default: http://127.0.0.1:4000)
bundle exec jekyll serve

# Start server with specific host/port
bundle exec jekyll serve --port 4000 --host 127.0.0.1

# Start server with live reload and incremental builds
bundle exec jekyll serve --livereload --incremental

# Start server in background
bundle exec jekyll serve --detach
```

### Building and Maintenance

```bash
# Build site for production
bundle exec jekyll build

# Clean generated files
bundle exec jekyll clean

# Update dependencies
bundle update

# Check site health
bundle exec jekyll doctor
```

### Stopping the Server

- **Interactive mode**: Press `Ctrl+C` in the terminal
- **Background mode**: Find and kill the process:
  ```bash
  ps aux | grep jekyll
  kill [process_id]
  ```

## Development Workflow

1. **Make changes** to any file (pages, layouts, styles)
2. **Save the file** - Jekyll will automatically rebuild
3. **Refresh browser** to see changes
4. **Check terminal** for any build errors

### File Structure

```
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
├── _includes/           # Reusable components
├── _sass/              # Styling (SCSS)
├── assets/             # CSS, JS, images
├── images/             # Site images and logos
├── index.md            # Home page
├── about.md            # About page
├── contact.md          # Contact page
├── help.md             # How Can I Help page
└── Gemfile             # Ruby dependencies
```

## Customization

### Content Updates
- **Home page**: Edit `index.md`
- **About page**: Edit `about.md`
- **Contact info**: Edit `contact.md`
- **Help page**: Edit `help.md`

### Images and Media
- **Logo files**: Replace in `images/logo/`
- **Hero image**: Replace `images/hero-placeholder.svg`
- **Team photos**: Add to `images/` and reference in about.md

### Site Configuration
- **Navigation**: Update `main_menu` in `_config.yml`
- **Contact info**: Update `contact` section in `_config.yml`
- **Site metadata**: Update `title`, `description` in `_config.yml`

## Deployment

This site is configured for **GitHub Pages**:

1. **Push changes** to the `main` branch
2. **GitHub automatically builds** and deploys the site
3. **Live site** updates within a few minutes

### Manual Deployment Check

```bash
# Build production version locally
bundle exec jekyll build --destination _site

# Serve production build
bundle exec jekyll serve --source _site --disable-disk-cache
```

## Troubleshooting

### Common Issues

**Server won't start**:
```bash
# Kill any existing processes
pkill -f jekyll
bundle exec jekyll serve
```

**Dependencies issues**:
```bash
# Clean and reinstall
bundle clean --force
bundle install
```

**Build errors**:
```bash
# Check for syntax errors
bundle exec jekyll doctor
bundle exec jekyll build --verbose
```

**Port already in use**:
```bash
# Use different port
bundle exec jekyll serve --port 4001
```

### Getting Help

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **Jekyll Serif Theme**: https://github.com/zerostaticthemes/jekyll-serif-theme
- **GitHub Pages**: https://docs.github.com/en/pages

## Contributing

1. **Fork** the repository
2. **Create feature branch**: `git checkout -b feature-name`
3. **Make changes** and test locally
4. **Commit changes**: `git commit -m "Description"`
5. **Push branch**: `git push origin feature-name`
6. **Create Pull Request**

## License

This project is maintained by Paw Pantry Mission Inc.

---

**Contact**: pawpantrymission@gmail.com | [Linktree](https://linktr.ee/pawpantrymission)