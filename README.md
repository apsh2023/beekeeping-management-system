# Beekeeping Management System

This project is an assignment submission for data modeling, featuring a comprehensive business design and data model for a modern beekeeping management system.

## 📖 Documentation Website

This project includes a professionally designed GitHub Pages website that showcases:

- **Business Design Analysis**: Comprehensive business requirements and system design
- **Data Model Specification**: Detailed database design with ERD and entity relationships
- **Implementation Guidelines**: Technical documentation and deployment instructions

### 🚀 View the Live Site

Once deployed, the documentation site will be available at your GitHub Pages URL.

## 🛠️ Quick Setup

### Deploy to GitHub Pages

1. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Select "GitHub Actions" as the source
   - The site will automatically deploy on pushes to main branch

2. **Add Your Content**:
   - Edit `business-design.md` with content from your `Business Design Project.docx`
   - Customize the data model in `data-model.md`
   - Update site configuration in `_config.yml`

### Local Development

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Visit http://localhost:4000
```

## 📁 Project Structure

```
├── index.md              # Home page
├── business-design.md    # Business design content (edit this!)
├── data-model.md         # Data modeling documentation
├── about.md              # Project information
├── _config.yml           # Site configuration
├── Gemfile              # Ruby dependencies
├── assets/css/          # Custom styling
├── .github/workflows/   # GitHub Actions for deployment
└── DEPLOYMENT.md        # Detailed deployment instructions
```

## 🎨 Features

- **Responsive Design**: Works on desktop and mobile devices
- **Professional Theme**: Business-appropriate styling with beekeeping-inspired colors
- **SEO Optimized**: Includes meta tags and sitemap generation
- **Fast Loading**: Optimized static site generation
- **Easy Content Management**: Simple Markdown editing

## 📝 Content Migration

To add content from your Business Design Project document:

1. Open `business-design.md`
2. Replace placeholder sections with content from your docx file
3. Use standard Markdown formatting for headers, lists, and emphasis
4. Commit and push changes to trigger automatic deployment

## 🔧 Customization

- **Colors & Styling**: Edit `assets/css/style.scss`
- **Navigation**: Update `header_pages` in `_config.yml`
- **Site Information**: Modify title, description, and URL in `_config.yml`

## 📚 Documentation

- [Deployment Instructions](DEPLOYMENT.md) - Detailed setup and deployment guide
- [GitHub Pages Docs](https://docs.github.com/en/pages) - Official GitHub Pages documentation
- [Jekyll Docs](https://jekyllrb.com/docs/) - Jekyll static site generator documentation

## 🎯 Academic Context

This project demonstrates:
- Advanced data modeling techniques
- Business analysis and requirements gathering
- Professional documentation practices  
- Modern web development and deployment workflows
- Version control and collaborative development

---

*For questions about deployment or customization, see [DEPLOYMENT.md](DEPLOYMENT.md) or check the repository's Issues section.*
