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

## Update & upgrade TermUX
```bash
pkg update -y && pkg upgrade -y
```
## SetUp Storage
```bash
termux-setup-storage
```
## Install [Proot-Distro](https://github.com/termux/proot-distro)
```bash
pkg install proot-distro -y
```
## Install Ubuntu CLI 
```bash
proot-distro install ubuntu-20.04
```
## Login in Ubuntu CLI
```bash
proot-distro login ubuntu-20.04
```
## Install sudo ( root / super user )
```bash
apt update -y && apt install sudo -y
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

## Update & upgrade Ubuntu
```bash
sudo apt update -y && sudo apt upgrade -y
```
## Install udisks2
```bash
sudo apt install udisks2 -y
```
## if [error](https://github.com/ShivaShirsath/Kubuntu-On-Android/issues)
```bash
rm -rf /var/lib/dpkg/info/*.postinst && sudo dpkg --configure -a
```

## Install Desktop ( Any one of following [ eg. xfce4 ] )

| DESKTOP | Info | `START-UP` |
| ---: | ---: | :--- |
| `ubuntu-desktop ` | Desktop |
| `ubuntu-gnome-desktop` | Gnome |
| `ubuntu-mate-desktop` | Mate | `/usr/bin/mate-session`
| `kubuntu-desktop` | Kubuntu | `/usr/bin/startkde` |
| `lxde` | Lightweight X11 |
| `xfce4` | X Forms Common | `/usr/bin/startxfce4` |

```bash
sudo apt install `DESKTOP`	
```

## Setting Virtual Network Computing ( VNC ) Server
```bash
sudo apt install tigervnc-standalone-server tigervnc-common tigervnc-xorg-extension tigervnc-viewer
```
## Run VNC Server & Open VNC Viewer
```bash
vncserver -xstartup `START-UP` -geometry 1800x900 :1
```
<!-- tigervncserver -xstartup /usr/bin/startkde -->
## Stop & Close
```bash
vncserver -kill :*
```
## Set password

## Install VNC Viewer 
<h1 align=center>
  <a href=https://play.google.com/store/apps/details?id=com.realvnc.viewer.android>
    ►
  </a>
</h1>

## How to use VNC Viewer ?
+ Open VNC Viewer
+ Enter Password
+ Set Quality to High 

<h1 align=center>& N joy !</h1>
