# Ubuntu setup
My ubuntu preferences put on paper


## Basic

``` bash
sudo apt update;  
sudo apt upgrade;  

sudo apt remove deja-dup rhythmbox thunderbird simple-scan;

sudo apt install vim curl cheese kazam backintime-qt rar ubuntu-restricted-extras build-essential \  
testdisk gparted openjdk-11-jdk steghide git gitg maven ffmpeg exfat-fuse exfat-utils flatpak \  
gimp gimp-plugin-registry gnome-tweaks apt-transport-https zsh zsh-common gnome-sushi \  
gnome-software-plugin-flatpak gnome-sound-recorder ca-certificates chrome-gnome-shell;

# Flathub

flatpak install flathub org.kde.digikam;
flatpak install flathub org.darktable.Darktable;
flatpak install flathub com.rawtherapee.RawTherapee;
flatpak install flathub org.kde.kdenlive;
flatpak install flathub com.spotify.Client;
flatpak install flathub com.github.johnfactotum.Foliate;

echo GTK_IM_MODULE=cedilla | sudo tee -a /etc/enironment

gsettings set org.gnome.desktop.peripherals.touchpad natural-scroll true
gsettings set org.gnome.desktop.peripherals.mouse natural-scroll true
gsettings set org.gnome.desktop.peripherals.touchpad two-finger-scrolling-enabled true
gsettings set org.gnome.shell.extensions.dash-to-dock autohide true
gsettings set org.gnome.shell.extensions.dash-to-dockdash-max-icon-size 32
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'
gsettings set org.gnome.desktop.interface show-battery-percentage true

```

## Dev

**- zsh**

https://www.addictivetips.com/ubuntu-linux-tips/switch-from-bash-to-zsh-on-linux/

**- IDEs**
``` bash
flatpak install flathub org.eclipse.Java;
flatpak install flathub com.google.AndroidStudio;
flatpak install flathub io.dbeaver.DBeaverCommunity;
flatpak install flathub com.visualstudio.code;
flatpak install flathub com.slack.Slack;

```

**- [Docker](https://docs.docker.com/engine/install/ubuntu)**

``` bash
sudo apt install gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

```

**- Node**

``` bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | zsh
nvm install v13.12.0
nvm use v13.12.0

```
#### By hand

- [Digikam](https://www.digikam.org/download)
- [VeraCrypt](https://www.veracrypt.fr/en/Downloads.html)
- [Chrome](http://www.google.com/intl/pt-BR/chrome/browser)
- [TeamViewer](http://www.teamviewer.com/pt/download/linux.aspx)
- Instalar drivers proprietários da placa de vídeo e wireless
- Habilitar software de terceiros empacotados pela canonical  
