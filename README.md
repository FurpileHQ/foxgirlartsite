# foxgirl.art

Coming soon page for **Axltte Nightfox**. Built and maintained by [RWD Co.](https://rwdco.us)

## Files

| File | Purpose |
|---|---|
| `index.html` | The page, with styles and scripts inline |
| `robots.txt` | Blocks known AI-training crawlers and allows regular search engines |
| `CNAME` | Custom domain for GitHub Pages |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Changing things

- **Colors:** edit the variables at the top of the `<style>` block (`--espresso`, `--latte`, etc.).
- **Contact email:** change `USER` in the contact script near the bottom of `index.html`.

## Art protection

Any element with a `data-art` attribute gets right-click and drag blocked, no long-press save on mobile, and a see-through shield over the image:

```html
<figure data-art>
  <img src="art/piece-web.jpg" alt="Description of the piece">
</figure>
```

Before uploading, apply Glaze/Nightshade to the files and post only low-resolution, watermarked web versions. Full-resolution files never go in this repo.

## Hosting

The site is temporarily on **GitHub Pages from a public repo**. Every file in the repo can be downloaded at full size, so **no artwork should be added until the site moves** to DigitalOcean, where server-level bot blocking and header controls are available.

### GitHub Pages setup

1. Push to `RWD-Co/foxgirl.art`.
2. Go to Settings, then Pages, and set it to deploy from branch `main` with folder `/ (root)`.
3. At the registrar, add four A records for `foxgirl.art`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. Add a CNAME record for `www` pointing to `rwd-co.github.io`.
4. Once DNS resolves, check **Enforce HTTPS**.
