# Pail

[![Tests](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml)
[![Excavator](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml)

I prefer to install all software in Windows via a package manager. If a trusted way is not readily available, scoop makes it really easy to create my own manifests. So this is a hodgepodge of software, all not otherwise available via a known/trusted repository for any of the Windows package managers (winget, Chocolatey, or scoop).

## How do I use this bucket?

First, [install the scoop package manager](https://github.com/ScoopInstaller/Install#readme).

Install this bucket:

```pwsh
scoop bucket add pail https://github.com/eclecticbouquet/pail
```

Install packages:

```pwsh
scoop install pail/<mainfest_name>
```

## How do I contribute new manifests?

To make a new manifest contribution to this or any bucket, please read the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md) and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests) wiki page.

## [License](https://github.com/eclecticbouquet/pail/blob/main/LICENSE)

This is free and unencumbered software, released into the public domain.
