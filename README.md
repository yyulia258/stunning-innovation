# Stunning Innovation

A modern, responsive knowledge sharing platform built with MkDocs and Material theme.
https://yyulia258.github.io/stunning-innovation/

## Features

- ✅ **Responsive Design** - Works seamlessly on all devices (mobile, tablet, desktop)
- ✅ **Accessible** - WCAG compliant with keyboard navigation and screen reader support
- ✅ **Light/Dark Mode** - Toggle between themes for comfortable reading
- ✅ **Gradient Color Theme** - Beautiful purple gradient design
- ✅ **Hero Images** - Eye-catching hero images on every page
- ✅ **Blog Support** - Easy to add new blog posts
- ✅ **GitHub Pages Ready** - Automated deployment via GitHub Actions

## Structure

- **Home Page** - Introduction and overview
- **Blog** - Articles and updates (easily add new posts)
- **Contact** - Get in touch page

## Local Development

### Prerequisites

- Python 3.x
- pip

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yyulia258/stunning-innovation.git
   cd stunning-innovation
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Serve the site locally:
   ```bash
   mkdocs serve
   ```

4. Open your browser and navigate to `http://127.0.0.1:8000`

## Building the Site

To build the static site:

```bash
mkdocs build
```

The built site will be in the `site/` directory.

## Adding Blog Posts

To add a new blog post:

1. Create a new markdown file in `docs/blog/posts/`
2. Add the post to the navigation in `mkdocs.yml` under `nav -> Blog -> Posts`
3. Update `docs/blog/index.md` to include a card for the new post

Example post structure:
```markdown
# Your Post Title

*Published: [Date]*

Your content here...
```

## Deployment

### GitHub Pages

The site automatically deploys to GitHub Pages when you push to the `main` branch via GitHub Actions.

Make sure GitHub Pages is enabled in your repository settings:
1. Go to Settings → Pages
2. Set Source to "GitHub Actions"

### Azure Static Web Apps

To deploy to Azure Static Web Apps, you can use the built site from the `site/` directory or configure Azure to run `mkdocs build`.

## Customization

### Colors

Edit `mkdocs.yml` to change the color scheme:
```yaml
theme:
  palette:
    primary: deep purple
    accent: purple
```

### Styling

Custom CSS is in `docs/stylesheets/extra.css`. Modify gradient colors and other styles there.

### Hero Images

Replace the SVG files in `docs/images/` with your own images (SVG, PNG, or JPG).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

See [LICENSE](LICENSE) file for details.
