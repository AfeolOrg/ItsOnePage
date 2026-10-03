# Publish without buying a domain

GitHub Pages provides a free `github.io` address. On GitHub Free, use a public repository: your website files will be publicly visible.

## Recommended: a site at your account address

1. Sign in to GitHub and create a public repository named `username.github.io`. Replace `username` with your actual GitHub username, in lowercase.
2. Upload your static website files. Put `index.html` at the repository root alongside its images, fonts, and other assets.
3. Add an empty `.nojekyll` file for a plain static site.
4. Open **Settings → Pages**. Select **Deploy from a branch**, then **main** and **/(root)**. Save.
5. Leave **Custom domain** empty. Open the published address shown by GitHub, normally `https://username.github.io/`.

Publication can take up to 10 minutes. Later commits to the selected branch publish updates automatically.

## Alternative: a project address

A repository named `my-site` can publish at `https://username.github.io/my-site/`.

For this layout, root-relative paths such as `/assets/Neuropol.otf` point outside the project. Adjust all image, font, stylesheet, script, icon, manifest, and navigation paths to include `/my-site/`, or use suitable relative paths. Check CSS `url()` values and manifest URLs too.

## If adapting the ItsOnePage demo

Use the presentation HTML and its referenced assets, rather than copying unrelated development files.

Replace the demo's content and SEO URLs with your own. Update canonical, social image, structured-data, robots, and sitemap URLs. Remove any `CNAME` file pointing to somebody else's domain. Cloudflare-specific `_redirects` and `_headers` do not configure GitHub Pages.

No domain purchase is required. GitHub Pages has usage limits and acceptable-use rules; check them before choosing it for your site. Hosting providers may process request data even when your site contains no visitor-tracking scripts.

This guide follows GitHub documentation. An ItsOnePage deployment on GitHub Pages has not yet been validated by this project.

## Official documentation

- [GitHub Pages quickstart](https://docs.github.com/en/pages/quickstart)
- [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [GitHub Pages limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)
