# Intent website

The official English and Simplified Chinese website for [Intent CRM](https://github.com/ZerothLab/intent-crm), maintained by ZerothLab.

**Website:** https://zerothlab.github.io/intent-crm-website/

This repository owns the public product website. Application code, releases, deployment instructions, and product documentation remain in [ZerothLab/intent-crm](https://github.com/ZerothLab/intent-crm). The live demo is not deployed; a hosting application is awaiting review.

## Preview

The site is static HTML, CSS, and JavaScript with no package dependencies, external fonts, or analytics.

```sh
python3 -m http.server 4178 --bind 127.0.0.1 --directory public
```

Open http://127.0.0.1:4178 . Before proposing changes, run `node --check public/site.js` and check both languages, narrow screens, links, keyboard navigation, command copy, and FAQ expansion in a browser.

## Contribute

Open a focused pull request. Preserve accurate product claims and links to published releases. Keep fictional data, the Fixture model, and simulated delivery visibly labeled. A screenshot is not a live demo. Do not add trackers, credentials, or real customer data.

Report website problems here; report product defects in the application repository. For sensitive findings, follow the [project security policy](https://github.com/ZerothLab/intent-crm/blob/main/.github/SECURITY.md).

## Publish

Pull requests run the website checks. Merges to protected `main` deploy only `public/` through GitHub Actions to GitHub Pages. The deployment uses the repository-provided token and OIDC; it has no Docker Hub credential or access to the application release secrets. Website changes do not build or publish application images.

## License

[Apache License 2.0](LICENSE).
