# VRM Revenue Dashboard — hosted frontend

Public hosting for the VRM Revenue Dashboard interface.

| File | |
|---|---|
| `index.html` | The live app. Talks to a Google Apps Script backend over HTTPS. |
| `demo.html` | Sample-data demo. No backend, nothing saved. |

Both files are **generated** — they are built from the private source repo by
`tools/build-pages.py`. Do not edit them here; edit the source and rebuild.

## What is and isn't here

This repository contains only the compiled frontend. There are no credentials,
no server code, and no data. Everything real — transactions, accounts, the audit
log — lives in a private Google Sheet reached through the Apps Script deployment.

Access is controlled by the app's own sign-in. Nothing in this repository grants
access to anything.

## Publishing

**Settings → Pages → Source: Deploy from a branch → Branch: `main` → Folder: `/ (root)`**

The app then serves at `https://<user>.github.io/<repo>/` and the demo at
`https://<user>.github.io/<repo>/demo.html`.
