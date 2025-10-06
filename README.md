# OnePageAPI - Zola Theme

A clean, minimal, single-page Zola theme for API and developer product landing pages.

## Features

- Single-page responsive design
- Minimal styling with blue color scheme
- Easy configuration via `config.toml`
- Ready for deployment

## Installation

```bash
zola init my-api-site
cd my-api-site
git clone https://github.com/VishalRashmika/OnePageAPI.git themes/OnePageAPI
```

Enable in `config.toml`:
```toml
theme = "OnePageAPI"
```

Start development:
```bash
zola serve
```

## Customization

**Change content:** Edit `templates/index.html`

**Change colors:** Replace `#2563eb` in `static/style.css` with your brand color

**Add logo:** Place image in `static/` and update header in `templates/index.html`

## Deployment

Build:
```bash
zola build
```

Deploy the `public/` directory to:
- **Netlify/Vercel:** Build command: `zola build`, Output: `public`
- **GitHub Pages:** `git subtree push --prefix public origin gh-pages`
- **Cloudflare Pages:** Build command: `zola build`, Output: `public`

## File Structure

```
apilanding/
├── config.toml
├── content/
│   └── _index.md
├── templates/
│   ├── base.html
│   └── index.html
└── static/
    └── style.css
```

## License

MIT License

## Links

- [Zola Documentation](https://www.getzola.org/documentation/)
- [Report Issues](https://github.com/VishalRashmika/OnePageAPI/issues)
