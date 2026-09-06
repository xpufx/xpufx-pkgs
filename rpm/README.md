# RPM Repository

Fedora/RHEL/CentOS RPMs via `dnf`/`yum`.

Add repo with low priority + includepkgs (only our packages visible):

```
sudo tee /etc/yum.repos.d/xpufx.repo <<'REPO'
[xpufx]
name=xpufx
baseurl=https://xpufx.github.io/xpufx-pkgs/rpm/$basearch
enabled=1
gpgcheck=0
priority=99
includepkgs=paseo* tone3000*
REPO
sudo dnf makecache
```
