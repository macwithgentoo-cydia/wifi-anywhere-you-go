# WiFi Anywhere You Go

A Cydia/APT repository for **WiFi Anywhere You Go**.

> **Status:** Repository setup is in progress. No installable package is published yet.

## Add this source in Cydia

Once GitHub Pages is enabled and the repository has deployed, add this source:

```
https://macwithgentoo-cydia.github.io/wifi-anywhere-you-go/repo/
```

In Cydia, open **Sources → Edit → Add**, then enter the URL above.

## Repository layout

- `repo/Release` — APT repository release metadata.
- `repo/Packages` — package index generated from published Debian packages.
- `repo/debs/` — location for compatible `.deb` packages.
- `.github/workflows/pages.yml` — builds the package index and deploys the site with GitHub Pages.

## Publishing packages

1. Build a Debian package (`.deb`) for the intended iOS jailbreak environment.
2. Add the package to `repo/debs/`.
3. Commit and push the change to `main`.
4. GitHub Actions will regenerate the package index and deploy the repository.

A package must match the device's jailbreak, iOS version, and CPU architecture. Hosting a package does not make it compatible with every device.

## Enable hosting

In this repository, open **Settings → Pages** and choose **GitHub Actions** as the build and deployment source. The deployment workflow will publish the repository root, keeping the Cydia source URL at the `/repo/` path.

## Current contents

This repository is being set up. It does not currently include an installable tweak or package.

## Licences

Each package should include its own licence and attribution. This README does not grant permission to redistribute third-party packages.
