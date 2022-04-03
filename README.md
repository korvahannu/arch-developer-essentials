## Required before you begin
> sudo pacman -S archlinux-keyring reflector
> 
> sudo reflector -c [COUNTRY] -a 6 --sort rate --save /etc/pacman.d/mirrorlist
> 
> sudo pacman -Syu

## Recommended essentials
> yay -S visual-studio-code-bin chromium gimp vlc pinta libreoffice-fresh intellij-idea-community-edition git nodejs-lts-gallium jdk-temurin pipewire pipewire-alsa pipewire-jack pipewire-media-session pipewire-pulse htop ntfs-3g cups hplip system-config-printer
> 
> When prompted to replace pulseaudio with pipewire, say Yes

#### Enable services
> systemctl enable --user pipewire pipewire-pulse pipewire-media-session

> sudo systemctl enable cups

## Other recommendations
> yay -S gedit virtualbox virtualbox-host-modules-arch pinta teamspeak3 webapp-manager zoom ttf-jetbrains-mono ttf-roboto qbittorrent

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

#### Great icons and theme sets
> yay -S matcha-gtk-theme mint-themes mint-themes-legacy papirus-icon-theme-git papirus-maia-icon-theme-git qogir-icon-theme we10x-icon-theme-git zorin-desktop-themes xcursor-simpleandsoft
