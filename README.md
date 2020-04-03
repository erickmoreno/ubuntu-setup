# Ubuntu setup

My ubuntu preferences put on paper
---

``` bash
sudo apt update;  
sudo apt upgrade;  

sudo apt remove deja-dup rhythmbox thunderbird;  

sudo apt install vim curl cheese kazam backintime-gnome rar ubuntu-restricted-extras build-essential \  
testdisk gparted openjdk-11-jdk steghide skype git gitg maven amarok ffmpeg exfat-fuse exfat-utils \  
gimp gimp-plugin-registry fbreader kdenlive gnome-tweaks fslint apt-transport-https;  

echo GTK_IM_MODULE=cedilla | sudo tee -a /etc/enironment;  

gsettings set org.gnome.desktop.peripherals.touchpad natural-scroll true;
gsettings set org.gnome.desktop.peripherals.touchpad two-finger-scrolling-enabled true;
gsettings set org.gnome.shell.extensions.dash-to-dock autohide true;  
gsettings set org.gnome.shell.extensions.dash-to-dockdash-max-icon-size 32;  

```
### vscode

``` bash
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg  
sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/  

sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt update;
sudo apt install code;

```

## OLD Version

O que fazer após uma instalação do zero do Ubuntu
- Instalar drivers proprietários da placa de vídeo e wireless
- Habilitar software de terceiros empacotados pela canonical  

Digikam:
  https://download.kde.org/stable/digikam/6.4.0/digikam-6.4.0-x86-64.appimage  
	sudo apt-add-repository ppa:philip5/extra  
	sudo apt install digikam showfoto  
	
NodeJS:

	curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
	sudo apt install nodejs

  https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions
	

Manualmente:
- TrueCrypt: https://www.grc.com/misc/truecrypt/truecrypt.htm
- Chrome: http://www.google.com/intl/pt-BR/chrome/browser
- Video plugin: https://www.google.com/chat/video
- Eclipse: http://www.eclipse.org/downloads/
- TeamViewer http://www.teamviewer.com/pt/download/linux.aspx
- Spotify https://www.spotify.com/br/download/linux/
- Rambox http://rambox.pro/#download
  
Aparência:
- Habilitar workspaces
- Remover hibernação quando baixar a tampa
- Remover som do cheese: /usr/share/sounds/freedesktop/stereo/camera-shutter...
  
Firefox:
- uBlock Origin
- login Account
