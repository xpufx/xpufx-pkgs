# Arch Repository

x86_64 packages (`pacman`).

Add to `/etc/pacman.conf`:

```
[xpufx]
Server = https://xpufx.github.io/xpufx-pkgs/arch/$arch
SigLevel = Optional TrustAll
```

Then `pacman -Sy`.
