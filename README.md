# Ubuntu setup

My ubuntu preferences put on paper
---

## Basic

``` bash
sudo apt update;  
sudo apt upgrade;  

sudo apt remove deja-dup rhythmbox thunderbird;  

sudo apt install vim curl cheese kazam backintime-qt rar ubuntu-restricted-extras build-essential \  
testdisk gparted openjdk-11-jdk steghide git gitg maven ffmpeg exfat-fuse exfat-utils flatpak \  
gimp gimp-plugin-registry fbreader kdenlive gnome-tweaks apt-transport-https zsh zsh-common darktable\  
gnome-software-plugin-flatpak;

echo GTK_IM_MODULE=cedilla | sudo tee -a /etc/enironment;  

gsettings set org.gnome.desktop.peripherals.touchpad natural-scroll true;
gsettings set org.gnome.desktop.peripherals.touchpad two-finger-scrolling-enabled true;
gsettings set org.gnome.shell.extensions.dash-to-dock autohide true;  
gsettings set org.gnome.shell.extensions.dash-to-dockdash-max-icon-size 32;  

```
#### Manual

- [VeraCrypt](https://www.veracrypt.fr/en/Downloads.html)  
- [Spotify](https://flathub.org/apps/details/com.spotify.Client)


## Dev

**- zsh**

https://www.addictivetips.com/ubuntu-linux-tips/switch-from-bash-to-zsh-on-linux/


**- vscode**

``` bash
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg  
sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/  

sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt update;
sudo apt install code;

```

**- Node**

``` bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | zsh
nvm install v13.12.0
nvm use v13.12.0

```
#### Flathub

``` bash
flatpak install flathub org.eclipse.Java
flatpak install flathub com.google.AndroidStudio
flatpak install flathub io.dbeaver.DBeaverCommunity
```

## Photo

``` bash
flatpak install flathub org.darktable.Darktable
``` 
- [Digikam](https://www.digikam.org/download)

## OLD Version

O que fazer após uma instalação do zero do Ubuntu
- Instalar drivers proprietários da placa de vídeo e wireless
- Habilitar software de terceiros empacotados pela canonical  
	
Manualmente:
- Chrome: http://www.google.com/intl/pt-BR/chrome/browser
- TeamViewer http://www.teamviewer.com/pt/download/linux.aspx
  
Aparência:
- Habilitar workspaces
- Remover hibernação quando baixar a tampa
