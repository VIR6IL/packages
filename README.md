# VIR6IL/packages

Binary cache and package repository for vir6il, served over GitHub Pages
at https://vir6il.github.io/packages/.

One independent Nix binary cache per package source, mirroring vir6il's
own `crates/system`/`crates/apps` split:

```
system/nix-cache-info, system/nar/*, system/*.narinfo
apps/nix-cache-info,   apps/nar/*,   apps/*.narinfo
packages.json          # shared index across both sources
```

Layout and publishing mechanism: `docs/stage-14.2-nix-cache-publish.md` in
the `vir6il` repo. Populated by `v6l package publish`/`v6l package
publish-all`/`v6l package publish-tool`; not edited by hand.
