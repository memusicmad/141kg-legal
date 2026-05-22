# 141kg-legal

Static hosting for the 141kg legal documents.

## Live URLs

- https://legal.141kg.com/terms/
- https://legal.141kg.com/privacy/

## Stack

Plain HTML, no build step, no framework. Served by GitHub Pages.

## Editing

Each document is a single self-contained HTML file:

- `terms/index.html`
- `privacy/index.html`

Edit the file, commit, push. GitHub Pages redeploys within a minute.

## Versioning

Each document carries a `Version` and `Effective from` date at the top.
Bump the version whenever the substance changes. The apps read these
version strings to decide whether to re-prompt users for acceptance.

## Tenant / Client app links

The Tenant and Client apps link to:

- `https://legal.141kg.com/terms/`
- `https://legal.141kg.com/privacy/`

Update the `TERMS_OF_SERVICE_URL` and `PRIVACY_POLICY_URL` constants in
each app to match.
