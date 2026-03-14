GitHub Pages deployment (using the `docs/` folder)

1. Place your site files in the `docs/` folder (this repository's `docs/index.html` is already prepared).
2. Commit and push to your default branch (usually `main`):

```bash
git add docs/index.html docs/DEPLOY.md
git commit -m "chore: add jwgreene.com single-page site"
git push origin main
```

3. Enable GitHub Pages for the repository:
- Go to the repository Settings → Pages
- Under "Source" choose the branch (e.g. `main`) and folder `docs/`
- Save — GitHub will publish the site at `https://<your-username>.github.io/<repo>/` or, if you configure a custom domain, at `https://www.jwgreene.com` after DNS updates.

4. Custom domain setup (optional):
- Create a DNS `A` record(s) or `CNAME` pointing `www.jwgreene.com` to GitHub Pages per GitHub's docs.
- Add the custom domain under Settings → Pages and verify.

5. Contact form: The example form in `docs/index.html` uses Formspree. Create a Formspree form to get an endpoint (https://formspree.io/) and update the `action` attribute in the HTML.
