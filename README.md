# andrew-andrada.github.io

Personal research portfolio site. Plain HTML/CSS, no build step, hosted on GitHub Pages.

## Local preview

Open `index.html` in a browser. That's it.

## Publish

1. Create a public repo on GitHub named exactly **`andrew-andrada.github.io`** (this exact name is what makes it a user site at the root domain).
2. Push the contents of this folder to that repo's `main` branch.
3. GitHub Pages auto-publishes user sites at `https://andrew-andrada.github.io/` within a minute or two.

```bash
cd "Portfolio Site"
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/andrew-andrada/andrew-andrada.github.io.git
git push -u origin main
```

## Updating

Edit `index.html`, commit, push. The site rebuilds automatically.

## Adding a case study

Each case study lives inside an `<article class="case">` block in `index.html`. Copy an existing one and edit:

- `<h3>` — case study title
- `.meta` — context line (role, org, year)
- `.tags` — short keyword chips
- `<dl>` — Question, Approach, Findings/Status, Outputs/Stack
- `.takeaway` — the UXR-translation paragraph
- `.case-links` (optional) — external links to source / live demos / publications
