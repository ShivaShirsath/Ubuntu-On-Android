<h1 align=center>Ubuntu On Android</h1>

+ **Update & upgrade TermUX [⇱](https://f-droid.org/packages/com.termux) / [►](https://play.google.com/store/apps/details?id=com.termux) & SetUp Storage**

  ```bash
  pkg update -y && pkg upgrade -y && termux-setup-storage
  ```
+ **Install [Proot-Distro](https://github.com/termux/proot-distro) & Install Ubuntu CLI & Login to Ubuntu**
  ```bash
  pkg install proot-distro -y && proot-distro install ubuntu && proot-distro login ubuntu
  ```
+ **Install sudo ( root / super user ) & Update & upgrade Ubuntu**
  ```bash
  apt update -y && apt install sudo -y && sudo apt update -y && sudo apt upgrade -y && sudo apt install -y apt-utils dialog git
  ``` 
<!--
+ Add User
```bash
adduser <UserName> && echo "<UserName> ALL=(ALL:ALL) ALL" >> /etc/sudoers
```
+ **Install udisks2**
```bash
rm -rf /var/lib/dpkg/info/*.postinst && sudo dpkg --configure -a && sudo apt install udisks2 -y && rm -rf /var/lib/dpkg/info/*.postinst && sudo dpkg --configure -a
``` -->

+ **Install Desktop ( Any one of following [ eg. xfce4 ] )**

  | DESKTOP | Information | START-UP |
  | ---: | :---: | --- |
  | `ubuntu-mate-desktop` | Mate | `mate-session`|
  | `kubuntu-desktop` | Kubuntu | `startplasma-x11` |
  | `lxde` | Lightweight X11 | `startlxde`
  | `xfce4 xfce4-goodies` | X Forms Common | `startxfce4` |
 
  ```bash
  sudo apt install -y `DESKTOP` 
  ```

+ **Setting Virtual Network Computing ( VNC ) Server**
  ```bash
  PWDx=$PWD && cd $HOME && rm -rf VNC && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx
  ```
+ **Use cammand to start or stop vnc**
  ```bash
  vnc 
  ```
<h2 align=center>
  <a href=https://play.google.com/store/apps/details?id=com.realvnc.viewer.android>
    Install VNC Viewer
  </a>
  <br>
  & N joy !
</h>

<h1 align=right>Bonus</h1>

```json
sudo apt install firefox -y # [ Mozilla ]
# Indian Fonts [ हिंदी देवनागरी मराठी ગુજરાતી ਪੰਜਾਬੀ ಕನ್ನಡ മലയാളം తెలుగు ] … etc etc
sudo apt install fonts-indic -y
# Emojies [ 😎 😃 ❤ 😍 😂 👍 😊 🎉 ] … etc etc
sudo apt install fonts-emojione -y
# [ java javac appletviewer jar ]
sudo apt install openjdk-8-jdk -y
```

[SS](Simple.md)

+ Install TermUX opener on Ubuntu
  ```bash
  wget https://raw.githubusercontent.com/ShivaShirsath/Ubuntu-On-Android/main/TermUX.desktop -O $HOME/TermUX.desktop && chmod +x $HOME/TermUX.desktop
  ```
