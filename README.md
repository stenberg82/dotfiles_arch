# dotfiles_arch
Dotfiles for ArchLinux (btw)
## System
- Paru - AUR
- Niri - Compositor
- Ly - Display manager
- Noctalia Shell
- Matugen

## Apps
- Fuzzel - app launcher
- Ghostty - terminal, replace Alacritty after install
- Yazi - CLI file manager
- VIM - editor
- Speicetify - Music
- Firefox - Browser
- Thunderbird - E-mail client

## Theme
- Catppuccin Macchiato

## Install
*Niri*
sudo pacman -Syu niri xwayland-satellite xdg-desktop-portal-gnome xdg-desktop-portal-gtk alacritty ly ghostty yazi firefox thunderbird vim spicetify
paru -S dms-shell-bin matugen wl-clipboard cliphist cava qt6-multimedia-ffmpeg
systemctl --user add-wants niri.service dms

*Noctalia shell*
paru -S noctalia-shell-git // develop
paru -S noctalia-shell // stable

*Ly*
systemctl enable ly@ttyX.service // X = 1-6
systemctl disable getty@ttyX.service /7 X = 1-6
