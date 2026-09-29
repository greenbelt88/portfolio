# Portfolio

My personal portfolio website.

**Live site:** https://greenbelt88.github.io/portfolio/

Built with plain HTML and CSS. There are no frameworks, build tools or JavaScript.

## Pages

| Page       | Path                      | Contents                                                               |
| ---------- | ------------------------- | ---------------------------------------------------------------------- |
| Home       | `index.html`            | Introduction, the tools I work with, and links to the rest of the site |
| About      | `about/index.html`      | Background and interests                                               |
| Experience | `experience/index.html` | Skills, training and certificates, work experience                     |
| Projects   | `projects/index.html`   | Projects with their tech stack and source code links                   |

## Project structure

```
├── index.html
├── about/
├── experience/
├── projects/
├── styles/
│   └── global.css       # Single stylesheet shared by every page
├── assets/
│   ├── docs/            # Certificate PDFs linked from the experience page
│   └── images/projects/ # Project screenshots and the no-preview placeholder
└── public/              # Favicons
```

Colours are defined as CSS variables at the top of `styles/global.css`, so changing one there updates it across the whole site.

## Running locally

Links point to folders (e.g. `projects/`) rather than `index.html`, so opening the files directly in a browser won't navigate correctly. Run a static server from the repository root instead, for example:

```
npx serve .
```

## Adding a project

Copy an existing `<article class="card project-card">` block in `projects/index.html`. Put its screenshot in `assets/images/projects/`, or use `no-preview-placeholder.svg` if there isn't one yet.
