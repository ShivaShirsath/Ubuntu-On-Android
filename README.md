<h1 align=center>Ubuntu On Android</h1>
<h1 align=center> 
  <a href=https://play.google.com/store/apps/details?id=com.termux>
    Install ►
  </a>
  /
  <a href=https://f-droid.org/packages/com.termux>
    ⇱ TermUX
  </a>
</h1>

+ **Update & upgrade TermUX**
```bash
pkg update -y
pkg upgrade -y
```
+ **SetUp Storage**
```bash
termux-setup-storage
```
+ **Install [Proot-Distro](https://github.com/termux/proot-distro)**
```bash
pkg install proot-distro -y
```
+ **Install Ubuntu CLI**
```bash
proot-distro install ubuntu
```
+ **Login in Ubuntu CLI**
```bash
proot-distro login ubuntu
```
+ **Install sudo ( root / super user )**
```bash
apt update -y
apt install sudo -y
```
<!--
## Add User
```bash
adduser <UserName>
```
## Add Permission to user
```bash
echo "<UserName> ALL=(ALL:ALL) ALL" >> /etc/sudoers
```
-->

+ **Update & upgrade Ubuntu**
```bash
sudo apt update -y
sudo apt upgrade -y
sudo apt install apt-utils -y
```
+ **Install udisks2**
```bash
sudo apt install udisks2 -y
```
+ **if [error](https://github.com/ShivaShirsath/Ubuntu-On-Android/issues)**
```bash
rm -rf /var/lib/dpkg/info/*.postinst
sudo dpkg --configure -a
```

+ **Install Desktop ( Any one of following [ eg. xfce4 ] )**

| DESKTOP | Info | START-UP |
| ---: | :---: | :--- |
| `ubuntu-desktop ` | Desktop |
| `ubuntu-gnome-desktop` | Gnome | `/usr/bin/gnome-session`
| `ubuntu-mate-desktop` | Mate | `/usr/bin/mate-session`
| `kubuntu-desktop` | Kubuntu | `/usr/bin/startkde` `/usr/bin/startplasma-x11` |
| `lxde` | Lightweight X11 | `/usr/bin/startlxde`
| `xfce4 xfce4-goodies` | X Forms Common | `/usr/bin/startxfce4` |

```bash
sudo apt install `DESKTOP`	
```

+ **Setting Virtual Network Computing ( VNC ) Server**
```bash
PWDx=$PWD
cd $HOME
rm -rf VNC
git clone https://github.com/ShivaShirsath/VNC.git
cd VNC
bash install
cd $PWDx
```
+ **Use cammand to start or stop vnc**
```bash
vnc 
```
+ **Install VNC Viewer**

<h1 align=center>
  <a href=https://play.google.com/store/apps/details?id=com.realvnc.viewer.android>
    ►
  </a>
</h1>
<h1 align=center>& N joy !</h1>
