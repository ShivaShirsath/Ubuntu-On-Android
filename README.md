<h1 align=center>Kubuntu On Android</h1>

## Install TermUX 
<h1 align=center>
  <a href=https://f-droid.org/packages/com.termux>
    ⇱
  </a><span> ‎ </span>
  <a href=https://play.google.com/store/apps/details?id=com.termux>
    ►
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
## Install Proot-Distro 
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
## Install sudo ( root/super user )
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

## Install desktop ( Any one of following [ eg. xfce4 ] )

| ‎         ‎ `DESKTOP` ‎         ‎  | Info
| ---: | ---:
| `ubuntu-desktop ` | Ubuntu Desktop Environment |
| `ubuntu-gnome-desktop` | Ubuntu Gnome Desktop Environment |
| `kubuntu-desktop` | Kubuntu Desktop Environment |
| `lxde` | Lightweight X11 Desktop Environment |
| `xfce4` | X Forms Common Environment |

```bash
sudo apt install `DESKTOP`	
```

## Setting Virtual Network Computing ( VNC ) Server
```bash
sudo apt install tigervnc-standalone-server tigervnc-common tigervnc-xorg-extension tigervnc-viewer
```
## Run VNC Server & Open VNC Viewer
```bash
tigervncserver -geometry 1800x900 :1
```
<!-- -xstartup /usr/bin/startkde -->
## Stop & Close
```bash
tigervncserver -kill :*
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
