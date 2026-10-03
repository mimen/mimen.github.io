---
repo_key: mimen.github.io
aliases: []
---

# mimen.github.io

A public GitHub Pages site publishing verification resources for a private Home Assistant installation. It contains a static landing page and the Tesla Fleet public key. It has no login, device controls, backend, or private credentials.

## Components

| Component | Path | What it is | Surfaces | Stack |
|---|---|---|---|---|
| Public verification site | `index.html`, `.well-known/`, `.nojekyll` | Static landing page and public-key assets served from the root of `main` by GitHub Pages. | web | static-html, github-pages |

## How the component operates

GitHub Pages publishes the files without Jekyll processing. The verification workflow checks PEM files with Python and OpenSSL to reject private keys and invalid public keys. Home Assistant uses the published resources but does not run in this repository.

## Repo-level gaps

The landing page links to `/home-assistant-app-info/`, which has no tracked page here. The repository has no deployment runbook or agent entry file.
