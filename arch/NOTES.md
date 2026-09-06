# Why no .pkg.tar.zst files here?

Packages exceed GitHub's 100MB git-file limit, so binaries live as assets
on the rolling `arch-x86_64-current` GitHub Release — which doubles as the
pacman `Server`. This directory only holds docs; `repo-add` runs in CI
against the release asset set.
