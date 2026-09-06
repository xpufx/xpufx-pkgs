# APT Repository

Debian/Ubuntu `.deb` pool.

Add repo + low-priority pin (so Debian main wins):

```
echo "deb [trusted=yes] https://xpufx.github.io/xpufx-pkgs/apt stable main" | sudo tee /etc/apt/sources.list.d/xpufx.list
cat <<'PIN' | sudo tee /etc/apt/preferences.d/99-xpufx
Package: *
Pin: origin xpufx.github.io
Pin-Priority: 100
PIN
sudo apt update
```

Only `paseo*` / `tone3000*` are in this repo.
