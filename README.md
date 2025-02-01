# Scoop Bucket Template

[![Tests](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml)
[![Excavator](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml)

Personally curated collection of Windows software, now scoopable.

## How do I use this bucket?

First, [install the scoop package manager](https://github.com/ScoopInstaller/Install#readme).

Install this bucket:

```pwsh
scoop bucket add pail https://github.com/eclecticbouquet/pail
```

Install apps:

```pwsh
scoop install pail/<manifestname>
```

## How do I contribute new manifests?

To make a new manifest contribution to this or any bucket, please read the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md) and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests) wiki page.

## Notes

Bucket test currently failing due to a bug with the bucket template, documented [here](https://github.com/ScoopInstaller/BucketTemplate/issues/18). Regardless, everything seems to be fuctioning.

## [License](https://github.com/eclecticbouquet/pail/blob/main/LICENSE)

This is free and unencumbered software, released into the public domain.
