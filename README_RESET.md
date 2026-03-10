This repository contains a reset/initialized Jekyll site in `new_site/`.

Workflow:
- A GitHub Actions workflow (`.github/workflows/jekyll_deploy.yml`) builds the site and deploys to `gh-pages` whenever the `reset-site` branch is pushed.

Next steps:
1. Review content in `new_site/`.
2. If OK, create a PR from `reset-site` to `master` and merge, or rename branches as desired.
