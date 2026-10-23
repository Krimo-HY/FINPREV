# FINPREV GitHub Pages site

This repository publishes the FINPREV dashboard as a static GitHub Pages site.

## Publish

1. In the GitHub repository, open **Settings → Pages** and set the build and deployment source to **GitHub Actions**.
2. Push these files to the `main` branch. The workflow in `.github/workflows/pages.yml` deploys the site automatically. It can also be run manually from the repository's **Actions** tab.
3. Open the site URL shown in the successful workflow run. The root page redirects to `dashboard.html`.

The dashboard reads `finprev_data.csv` from the same directory. To update the data, replace the CSV while keeping its semicolon delimiter and expected column headers, then commit and push the change to `main`. The page is redeployed automatically.

The site and CSV are public. Do not publish confidential or restricted data here.
