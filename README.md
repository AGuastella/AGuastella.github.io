# AGuastella.github.io

Personal portfolio site, served via GitHub Pages at https://aguastella.github.io.

Plain HTML/CSS, no build step, no dependencies.

## Structure

```
index.html          home: about, projects, publications
projects/
  talia.html         project writeup
  sparsyfed.html      project writeup
style.css            shared stylesheet (light/dark via prefers-color-scheme)
.nojekyll            disables Jekyll processing on GitHub Pages
```

## Adding a project

1. Copy `projects/sparsyfed.html` as a starting point.
2. Add a `<a class="card">` entry linking to it from `index.html`'s `#projects` section.

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```sh
python -m http.server 8000
```

## Deploy

Push to `main`. GitHub Pages serves the repo root automatically once Pages is
enabled in the repo settings (Settings &rarr; Pages &rarr; Source: `main` branch, `/` root).
