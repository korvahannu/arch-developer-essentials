## Required before you begin
> sudo pacman -S archlinux-keyring reflector
> 
> sudo reflector -c [COUNTRY] -a 6 --sort rate --save /etc/pacman.d/mirrorlist
> 
> sudo pacman -Syu

## Recommended essentials
> yay -S gedit visual-studio-code-bin chromium gimp virtualbox virtualbox-host-modules-arch vlc pinta libreoffice-fresh intellij-idea-community-edition teamspeak zoom webapp-manager git nodejs-lts-gallium jdk-temurin pipewire pipewire-alsa pipewire-jack pipewire-media-session pipewire-pulse htop pfetch neofetch ttf-ms-win10-auto ttf-jetbrains-mono ttf-roboto ntfs-3g qbittorrent cmatrix cups hplip system-config-printer

#### Enable services:
> systemctl enable --user pipewire pipewire-pulse pipewire-media-session

> sudo systemctl enable cups 

#### Rust
> curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

#### Flatkpak and Steam
> yay -S flatpak
> 
> flatpak --user remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
> 
> flatpak --user install flathub com.valvesoftware.Steam
> 
> flatpak run com.valvesoftware.Steam

#### Make bash auto-completion case insensitive
> echo 'set completion-ignore-case On' | sudo tee -a /etc/inputrc

#### xfce4 whiskermenu super-key fix
> set a keyboard shortcut for command xfce4-popup-whiskermenu at keybinding of L_Shift + L_CTRL, L_ALT +Super + D
> 
> Install xcape with sudo pacman -S xcape
> 
> Enable binding on terminal with command: xcape -e 'Super_L=Shift_L|Control_L|Alt_L|Super_L|D'
> 
> Add the command mentioned above to be run on startup
