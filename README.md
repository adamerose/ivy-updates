# Ivy update feed

This public repository contains Ivy's signed Stable and Edge update metadata. Windows installers are immutable GitHub Release assets; the Pages site contains only small metadata and a minimal index. Ivy source code and signing keys do not belong here.

- [Download the current Stable installer](https://adamerose.github.io/ivy-updates/stable/)
- [Download the current Edge installer](https://adamerose.github.io/ivy-updates/edge/)

Copy this template into the empty public `adamerose/ivy-updates` repository, enable GitHub Pages through Actions, and protect `main`. Before creating any Release, run Ivy's `pnpm release:provision-updates` preflight to enable [immutable Releases](https://docs.github.com/en/rest/repos/repos#enable-immutable-releases); GitHub applies the setting only to future Releases. The private source repository may write here only through a fine-grained `IVY_UPDATES_TOKEN` limited to this repository. Provisioning needs Administration write permission; normal publication needs Administration read and Contents write.
