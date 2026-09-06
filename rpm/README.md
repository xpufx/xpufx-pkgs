# RPM Repository

Fedora/RHEL/CentOS RPMs via `dnf`/`yum`.

Add repo:
```
sudo tee /etc/yum.repos.d/xpufx.repo <<'REPO'
[xpufx]
name=xpufx
baseurl=https://xpufx.github.io/xpufx-pkgs/rpm/$basearch
enabled=1
gpgcheck=0
REPO
sudo dnf makecache
```
