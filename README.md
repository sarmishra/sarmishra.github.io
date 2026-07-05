# Saroj Mishra — Personal Website

Personal portfolio and research homepage.
Built as a static site with client-side Markdown rendering — no build step required.

🌐 **Live:** https://sarmishra.github.io/

## About

I'm an AI/LLM engineer and researcher based in Dallas, Texas. I build agentic AI systems, RAG pipelines, and trustworthy AI infrastructure, and I publish research on secure agent architectures, MCP security, and hallucination mitigation. Currently at MaxModus. Previously at Goldman Sachs.

## Sections on the site

- **About** — background, current work, education, and research focus
- **Experience** — professional history
- **Publications** — research on agentic AI, LLM security, MCP, and RAG
- **Achievements** — awards and certifications

## Stack

Vanilla HTML + Bootstrap 5 + client-side Markdown rendering via [marked.js](https://marked.js.org/) and [js-yaml](https://github.com/nodeca/js-yaml). MathJax for equations. No build step, no framework, no server-side rendering.

Based on [StartBootstrap's New Age](https://github.com/StartBootstrap/startbootstrap-new-age) template.

## Structure

```
sarmishra.github.io/
├── index.html                    # Page shell, section anchors, footer links
├── contents/                     # All editable content
│   ├── config.yml                # Site title, tagline, copyright
│   ├── home.md                   # About section
│   ├── experience.md             # Roles + brief impact summaries
│   ├── publications.md           # Papers
│   └── achievements.md           # Awards + certifications
└── static/
    ├── assets/
    │   ├── favicon.ico           # SM monogram favicon
    │   └── img/
    │       ├── background.jpeg   # Hero band (network graph, 1920x400)
    │       └── photo.png         # Profile photo
    ├── css/
    │   ├── styles.css            # Bootstrap base
    │   └── main.css              # Custom overrides + section gradients
    └── js/
        ├── scripts.js            # Section loader, YAML config, scrollspy
        ├── bootstrap.bundle.min.js
        ├── marked.min.js
        └── js-yaml.min.js
```

## Local development

Clone and serve — no build step:

```bash
git clone https://github.com/sarmishra/sarmishra.github.io.git
cd sarmishra.github.io
python3 -m http.server 8000
# Visit http://localhost:8000
```

Any static server works. `fetch()` from `file://` URLs is blocked in most browsers, so you must serve rather than open `index.html` directly.

## Editing content

- **Change tagline, title, or copyright** → edit `contents/config.yml`. Each YAML key must exactly match a DOM element `id` in `index.html`; unrecognized keys are silently ignored (see `scripts.js` line 40).
- **Edit an existing section's text** → edit the matching `contents/<name>.md`.
- **Add a new section** requires **three coordinated edits**:
  1. Create `contents/<newname>.md`
  2. Add `'<newname>'` to the `section_names` array in `static/js/scripts.js`
  3. Add a `<section id="<newname>">` block in `index.html` containing a `<div id="<newname>-md">` mount point and, optionally, a `<h2 id="<newname>-subtitle">` header
  
  Skipping any one of these causes the section to silently not render.

## Deployment

GitHub Pages auto-deploys from `main` on push. No CI, no build.

## License

MIT. See [LICENSE](LICENSE).
