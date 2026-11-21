# Portfolio and blog

A [Hugo](https://gohugo.io) site using the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme (copied into `themes/PaperMod`, MIT licensed).

## Run locally

Install Hugo (extended, v0.158.0 or newer), then:

```bash
hugo server -D      # preview at http://localhost:1313, including drafts
```

## Write

```bash
hugo new posts/my-post.md        # blog post
hugo new projects/my-project.md  # portfolio project
```

Set `draft: false` in the front matter to publish.

## Customize

Edit `hugo.yaml`: site title, author, intro text on the home page, social links, menu. Edit `content/about.md` for the About page.

## Deploy (GitHub Pages)

1. Push to a GitHub repo with a `main` branch.
2. In the repo: Settings, Pages, Source: **GitHub Actions**.
3. Every push to `main` builds and publishes via `.github/workflows/hugo.yaml`.

For a custom domain, add it under Settings, Pages, and set `baseURL` in `hugo.yaml`.
