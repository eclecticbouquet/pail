# Pail

[![Tests](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/ci.yml)
[![Excavator](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml/badge.svg)](https://github.com/eclecticbouquet/pail/actions/workflows/excavator.yml)
[![Maintained](https://img.shields.io/badge/maintained-actively-green.svg)](https://github.com/eclecticbouquet/pail)

This is a package repository for [Scoop](https://scoop.sh/), a Windows package manager. Scoop package repositories are called "buckets". There are a few official/trusted buckets, but users can create their own with a simple git repository. This is mine, created so that I can easily create my own manifests if needed. I use it for software that isn't already available via a **trusted** repository for any of the main Windows package managers (winget, Chocolatey, or scoop).

Browse the packages in this bucket [here](https://scoop.sh/#/apps?q=%22https%3A%2F%2Fgithub.com%2Feclecticbouquet%2Fpail%22&o=false).

## ⚠️ Security Warning: Review Manifests Before Installing

Scoop **runs PowerShell scripts from manifests automatically**, even if your system has script execution restrictions. Malicious or compromised manifests could execute harmful commands without your knowledge. To mitigate this risk:

✅ **Only use trusted buckets.**

Stick to TRUSTED and actively maintained sources like ```main``` and ```extras```. If using third-party buckets, like this one, review their contents regularly.

✅ **Check manifests before installing and updating packages.**

To check manifests from the scoop CLI, run:

```pwsh
scoop cat <package>
```
Critically examine the ```pre_install```, ```post_install```, or ```installer``` sections, as these can run scripts.

✅ **Verify the software and it's source.**

Aside from the manifest, you need to make sure you trust the software itself. Look into the vendor, and make sure that the manifest is downloading the package directly from them.

## How do I use this bucket?

First, [install the scoop package manager](https://github.com/ScoopInstaller/Install#readme).

Install this bucket:

```pwsh
scoop bucket add pail https://github.com/eclecticbouquet/pail
```

Install packages:

```pwsh
scoop install pail/<package>
```

## How do I contribute new manifests?

To make a new manifest contribution to this or any bucket, please read the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md) and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests) wiki page.

## [License](https://github.com/eclecticbouquet/pail/blob/main/LICENSE)

This is free and unencumbered software, released into the public domain.
