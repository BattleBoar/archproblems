# archproblems

sudo rm -rf /etc/pacman.d/gnupg/ && \
sudo pacman-key --init && \
sudo pacman-key --populate archlinux cachyos && \
sudo pacman -Syy archlinux-keyring

sudo pacman-key --recv-keys F3B607488DB35A47 --keyserver keyserver.ubuntu.com
sudo pacman-key --lsign-key F3B607488DB35A47

sudo pacman -U https://mirror.cachyos.org/repo/x86_64/cachyos/cachyos-keyring-latest-any.pkg.tar.zst
sudo pacman -U https://mirror.cachyos.org/repo/x86_64/cachyos/cachyos-repo-1-1-any.pkg.tar.zst
