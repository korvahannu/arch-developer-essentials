## Required before you begin
> sudo pacman -S archlinux-keyring
> sudo pacman -Syu

## Recommended essentials
yay -S gedit visual-studio-code-bin chromium gimp virtualbox virtualbox-host-modules-arch vlc pinta libreoffice-fresh intellij-idea-community-edition teamspeak zoom webapp-manager git nodejs-lts-gallium jdk-temurin pipewire pipewire-alsa pipewire-jack pipewire-media-session pipewire-pulse htop pfetch neofetch ttf-ms-win10-auto ttf-jetbrains-mono ttf-roboto ntfs-3g qbittorrent cmatrix

#### Enable pipewire:
systemctl enable pipewire pipewire-pulse pipewire-media-session

#### Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

#### Flatkpak and Steam
yay -S flatpak
flatpak --user remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
flatpak --user install flathub com.valvesoftware.Steam
flatpak run com.valvesoftware.Steam
