## Components of a Coding Agent

This presentation is based on the great article [Components of A Coding Agent](https://magazine.sebastianraschka.com/p/components-of-a-coding-agent) by Sebastian Raschka.

## Static Site Setup

This repo is set up to publish as a static site on GitHub Pages.

- `index.html` is the live presentation entrypoint.
- `Components of a Coding Agent.html` is a compatibility redirect to `index.html`.
- `.github/workflows/deploy-pages.yml` deploys the site with GitHub Actions.
- `.nojekyll` ensures GitHub Pages serves the repo as plain static files.

## GitHub Pages URL

Live presentation:

- https://svdoever.github.io/Components-of-a-Coding-Agent/

After enabling GitHub Pages with GitHub Actions, the site URL will usually be:

- User or org site repo: `https://<owner>.github.io/`
- Project site repo: `https://<owner>.github.io/<repo>/`

For this repository, the published URL is `https://svdoever.github.io/Components-of-a-Coding-Agent/`.

## Local Preview

Because this is a plain static site, you can preview it locally with any simple HTTP server from the repo root.

PowerShell with Python:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Publishing

1. Push the repository to GitHub.
2. In repository settings, open Pages.
3. Set the source to GitHub Actions if it is not already selected.
4. Push to `main` or `master`, or run the workflow manually.
