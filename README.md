<h1 align=center>Ubuntu KDE On Android</h1>

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
## if [error](https://github.com/ShivaShirsath/Ubuntu-KDE-On-Android/issues)

## Install desktop with mate & VNC-server
```bash
sudo apt install kubuntu-desktop tigervnc-standalone-server 
```
## Run & Open 
```bash
tigervncserver -xstartup /usr/bin/startkde -geometry 1800x900 :1
```
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
