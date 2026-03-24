# GitHub Pages Deployment Instructions

## Automatic Deployment Setup

### 1. Enable GitHub Pages

1. Go to your GitHub repository settings
2. Scroll down to the "Pages" section
3. Under "Source", select "GitHub Actions"
4. The workflow will automatically trigger on pushes to the main branch

### 2. Repository Settings

Make sure your repository has the following settings:
- **Repository name**: Can be any name, but if named `username.github.io`, it will be available at that URL
- **Visibility**: Can be public or private (GitHub Pages works with private repos on paid plans)

### 3. Branch Protection (Optional but Recommended)

- Set up main branch protection to require pull request reviews
- This ensures quality control before deployment

## Manual Deployment

If you prefer to deploy manually:

```bash
# Install dependencies
bundle install

# Build the site locally
bundle exec jekyll build

# Serve locally for testing
bundle exec jekyll serve
```

## Site URLs

Once deployed, your site will be available at:
- **Custom repository**: `https://username.github.io/repository-name`
- **User site**: `https://username.github.io` (if repository is named `username.github.io`)

## Updating Content

### From Your Business Design Document

1. Open your `Business Design Project.docx` file
2. Copy the content section by section
3. Edit the [business-design.md](business-design.md) file
4. Replace the placeholder sections with your actual content
5. Commit and push changes

### Adding New Pages

1. Create new `.md` files in the root directory
2. Add front matter:
   ```yaml
   ---
   layout: page
   title: Your Page Title
   permalink: /your-page-url/
   ---
   ```
3. Add the page to navigation in `_config.yml` under `header_pages`

### Customizing Styling

- Edit [assets/css/style.scss](assets/css/style.scss) to modify colors, fonts, and layout
- The current theme uses a beekeeping-inspired color scheme (browns and golds)

## File Structure

```
├── _config.yml           # Jekyll configuration
├── Gemfile              # Ruby dependencies
├── index.md             # Home page
├── business-design.md   # Business design content
├── data-model.md        # Data modeling content  
├── about.md             # About page
├── assets/
│   └── css/
│       └── style.scss   # Custom styling
└── .github/
    └── workflows/
        └── pages.yml    # GitHub Actions deployment
```

## Troubleshooting

### Build Failures

1. Check the Actions tab in your GitHub repository
2. Review build logs for specific errors
3. Common issues:
   - Invalid YAML front matter
   - Missing dependencies in Gemfile
   - Markdown syntax errors

### Local Development

```bash
# Install Jekyll locally
gem install bundler jekyll

# Navigate to your project directory
cd your-repository

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve --livereload
```

### Domain Configuration (Optional)

To use a custom domain:
1. Add a `CNAME` file with your domain name
2. Configure DNS settings with your domain provider
3. Update `url` in `_config.yml`

## Support

For issues with GitHub Pages deployment:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- Check the repository's Issues tab for common problems