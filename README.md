## bspwm  
  
A tiling window manager based on binary space partitioning  
  
Automatic install/update:

```shell
bash -c "$(curl -LSs https://github.com/desktopmgr/bspwm/raw/main/install.sh)"
```

Manual install:
  
requires:

Debian based:

```shell
apt install bspwm libnotify-bin catfish slimlock acpi-support wireless-tools gtk2-engine-murrine xfce4-terminal firefox xfce4-power-manager volumeicon-alsa xscreensaver policykit-1-gnome gnome-settings-daemon network-manager-gnome conky polybar xbindkeys tint2
```  

Fedora Based:

```shell
yum install xfce4-power-manager gtk2-murrine-engine acpid wireless-tools xfce4-terminalfirefox  volumeicon xscreensaver policykit-1-gnome gnome-settings-daemon network-manager-gnome polybar xbindkeys tint2
```  

Arch Based:

```shell
pacman -S bspwm gtk-engine-murrine xfce4-power-manager acpi wireless-tools xfce4-terminal firefox volumeicon xscreensaver polkit-gnome gnome-settings-daemon network-manager-applet conky tint2 xbindkeys polybar
```  

MacOS:  

```shell
brew install
```
  
```shell
mv -fv "$HOME/.config/bspwm" "$HOME/.config/bspwm.bak"
git clone https://github.com/desktopmgr/bspwm "$HOME/.config/bspwm"
```
  
<p align=center>
  <a href="https://wiki.archlinux.org/index.php/bspwm" target="_blank" rel="noopener noreferrer">bspwm wiki</a>  |  
  <a href="https://github.com/baskerville/bspwm" target="_blank" rel="noopener noreferrer">bspwm site</a>
</p>  
