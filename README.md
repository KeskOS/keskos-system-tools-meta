# keskos-system-tools-meta

Meta package for curated KeskOS system utilities and customization tools

This repository contains the standalone Arch package source for `keskos-system-tools-meta`.

## Contents

- `PKGBUILD`
- `files/` for packaged assets, scripts, themes, or source snapshots where needed

## Build

```bash
makepkg -s --noconfirm
```

## Package Metadata

- Version: `0.1.0`
- Architectures: `any`

This repo is intended to be consumed by the KeskOS package build server and can also be built locally with standard Arch tooling.
