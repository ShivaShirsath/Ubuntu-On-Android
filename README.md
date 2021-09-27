<h1 align=center>Ubuntu On Android</h1>

<ul>
  <li>
    <strong>
      Update & upgrade TermUX
      <a href=https://f-droid.org/packages/com.termux>
        ⇱ 
      </a>
      /
      <a href=https://play.google.com/store/apps/details?id=com.termux>
        ►
      </a>
      & SetUp Storage
    </stong>
  </li>
</ul> 

```bash
pkg update -y && pkg upgrade -y &&ntermux-setup-storage
```
+ **Install [Proot-Distro](https://github.com/termux/proot-distro) & Install Ubuntu CLI & Login to Ubuntu**
```bash
pkg install proot-distro -y && proot-distro install ubuntu && proot-distro login ubuntu
```
+ **Install sudo ( root / super user ) & Update & upgrade Ubuntu**
```bash
apt update -y && apt install sudo -y && sudo apt update -y && sudo apt upgrade -y && sudo apt install apt-utils -y
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

| DESKTOP | Info | START-UP |
| ---: | :---: | --- |
| `ubuntu-mate-desktop` | Mate Desktop | `mate-session`|
| `kubuntu-desktop` | Kubuntu Desktop | `startplasma-x11` |
| `lxde` | Lightweight X11 Desktop Environment | `startlxde`
| `xfce4 xfce4-goodies` | X Forms Common Environment | `startxfce4` |
 
```bash
sudo apt install -y `DESKTOP` 
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

<h1 align=center> Install VNC Viewer => 
  <a href=https://play.google.com/store/apps/details?id=com.realvnc.viewer.android>
    Play Store
  </a>
</h1>
<h1 align=center>& N joy !</h1>
