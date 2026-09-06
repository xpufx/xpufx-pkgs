# Arch Repository

x86_64 packages (`pacman`). Only `paseo-*` / `tone3000-*` — no system shadowing.

Add **last** in `/etc/pacman.conf` (after [core]/[extra]):

```
[xpufx]
Server = https://xpufx.github.io/xpufx-pkgs/arch/$arch
SigLevel = Optional TrustAll
```

Then:

```
sudo pacman -Sy
pacman -S xpufx/paseo-cli-git
```

Only our packages exist in [xpufx]; `pacman -S bash` still comes from core.
