# keskos-system-tools-meta

`keskos-system-tools-meta` pulls in the system utilities and customization helpers recommended by KeskOS.

## What this is

This repository builds a pacman meta package. The package itself is empty at runtime and exists only to pull in a curated group of packages through dependencies.

## Role in KeskOS

Optional meta package group.

## Package name

```txt
Package: keskos-system-tools-meta
Repo: [keskos]
Architecture: any
```

## What it installs or provides

- Installs no runtime files beyond pacman metadata.
- Pulls in its software set entirely through `depends` (and optional `optdepends` where present).

## Commands and launchers

- This package does not install commands, GUI launchers, config files, logs, or systemd units directly.

## Config, logs, and state

- Configuration and logs belong to the packages pulled in by this meta package, not to the meta package itself.

## Dependencies

- Current hard dependencies: `btop`, `fastfetch`, `gparted`, `htop`, `kate`, `kdeconnect`, `papirus-icon-theme`, `partitionmanager`, `qt6ct`, and `timeshift`.
- Build with `makepkg -s --noconfirm`.

## Build

```bash
makepkg -s --noconfirm
```

## Packaging notes

- Keep the package name stable so it can be referenced cleanly by installer presets and higher-level meta packages.

## Troubleshooting

- If installation fails, the problem is usually in one of the dependency packages or in repository availability, not in the empty meta package itself.

## Docs website export notes

- Docs site usage: package-group overview plus the dependency list from this README.
