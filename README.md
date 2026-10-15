# DaZui Scoop Bucket

[![Tests](https://github.com/DaZui/scoop/actions/workflows/ci.yml/badge.svg)](https://github.com/DaZui/scoop/actions/workflows/ci.yml) [![Excavator](https://github.com/DaZui/scoop/actions/workflows/excavator.yml/badge.svg)](https://github.com/DaZui/scoop/actions/workflows/excavator.yml)

Personal bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## Apps

| App | Description |
| --- | --- |
| [Bettbox](bucket/bettbox.json) | Cross-platform network proxy client based on Mihomo. |
| [usque](bucket/usque.json) | Open-source reimplementation of the Cloudflare WARP client's MASQUE protocol. |
| [usque-app](bucket/usque-app.json) | High-performance cross-platform GUI for Cloudflare WARP client's MASQUE protocol. |

## How do I add a new manifest?

1. Copy `bucket/app-name.json.template` to `bucket/<app-name>.json`.
2. Fill in the blanks, following the [App
   Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests) wiki page.
3. Commit and push. The Excavator workflow keeps `version`, `url` and `hash`
   up to date afterwards.

## How do I install these manifests?

After manifests have been committed and pushed, run the following:

```pwsh
scoop bucket add DaZui https://github.com/DaZui/scoop
scoop install DaZui/usque
```

## How do I contribute new manifests?

To make a new manifest contribution, please read the [Contributing
Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
wiki page.
