# Ubuntu setup

My ubuntu preferences put on paper

## Basic

``` bash
sudo apt update && sudo apt upgrade;  

sudo apt remove deja-dup rhythmbox thunderbird simple-scan;

sudo apt install vim curl cheese kazam backintime-qt rar ubuntu-restricted-extras \  
testdisk gparted steghide ffmpeg exfat-fuse exfat-utils flatpak gnome-tweaks \ 
apt-transport-https zsh zsh-common gnome-sushi gnome-software-plugin-flatpak \ 
gnome-sound-recorder ca-certificates chrome-gnome-shell;

flatpak install flathub \
 com.spotify.Client \
 com.github.debauchee.barrier \ 
 com.github.johnfactotum.Foliate;

echo GTK_IM_MODULE=cedilla | sudo tee -a /etc/environment

gsettings set org.gnome.desktop.peripherals.touchpad natural-scroll true
gsettings set org.gnome.desktop.peripherals.mouse natural-scroll true
gsettings set org.gnome.desktop.peripherals.touchpad two-finger-scrolling-enabled true
gsettings set org.gnome.shell.extensions.dash-to-dock autohide true
gsettings set org.gnome.shell.extensions.dash-to-dockdash-max-icon-size 32
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'
gsettings set org.gnome.desktop.interface show-battery-percentage true

```

## Graphics

``` bash
sudo apt install gimp gimp-plugin-registry;

flatpak install flathub org.kde.digikam \ 
 com.rawtherapee.RawTherapee \ 
 org.darktable.Darktable \ 
 org.kde.kdenlive;

```

## Dev

``` bash
sudo apt install build-essential openjdk-11-jdk git gitg maven;

flatpak install flathub org.eclipse.Java \ 
 io.dbeaver.DBeaverCommunity \ 
 com.google.AndroidStudio \ 
 com.getpostman.Postman \ 
 com.visualstudio.code \ 
 com.slack.Slack;

```

**- zsh**

https://www.addictivetips.com/ubuntu-linux-tips/switch-from-bash-to-zsh-on-linux/

**- [Docker](https://docs.docker.com/engine/install/ubuntu)**

``` bash
sudo apt install gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update && sudo apt install docker-ce docker-ce-cli containerd.io

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
- [Stacer](https://github.com/oguzhaninan/Stacer/releases)
- [TeamViewer](http://www.teamviewer.com/pt/download/linux.aspx)
- Install proprietary drivers for video card and wireless
- Habilitar software de terceiros empacotados pela canonical  
