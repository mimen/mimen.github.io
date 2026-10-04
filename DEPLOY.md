---
deployment_status: partial
deployment_last_assessed: 2026-10-03
deployment_targets:
  - component: Public verification site
    where: github-pages
    detail: GitHub Pages publishes the root of main without Jekyll processing.
    url: https://mimen.github.io/
---

# Deployment

GitHub Pages publishes the static files from the root of `main`, as recorded in `PROJECT.md` and the repository's Pages configuration. `.nojekyll` disables Jekyll processing. `.github/workflows/verify.yml` checks public PEM keys on pushes and pull requests. The repository has no scripted deployment or destination verification command.
