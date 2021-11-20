<h1 align=center>Ubuntu On Android</h1>

**TermUX → [Download](https://f-droid.org/packages/com.termux) / [Install](https://play.google.com/store/apps/details?id=com.termux)**
+ **Update & upgrade & SetUp Storage**
  ```bash
  pkg update -y && pkg upgrade -y && termux-setup-storage
  ```
+ **Install [Proot-Distro](https://github.com/termux/proot-distro) & Ubuntu CLI & Login to CLI**
  ```bash
  pkg install proot-distro -y && proot-distro install ubuntu && proot-distro login ubuntu
  ```
+ **Install sudo ( root / super user ) & Update & Upgrade**
  ```bash
  apt update -y && apt install sudo -y && sudo apt update -y && sudo apt upgrade -y && sudo apt install -y apt-utils dialog git wget
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
<details>
<summary>Desktops</summary>
<table>
<thead>
<tr>
<th style="text-align:right">DESKTOP</th>
<th style="text-align:center">Info</th>
<th>START-UP</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:right"><code>ubuntu-mate-desktop</code></td>
<td style="text-align:center">Mate</td>
<td><code>mate-session</code></td>
</tr>
<tr>
<td style="text-align:right"><code>kubuntu-desktop</code></td>
<td style="text-align:center">Kubuntu</td>
<td><code>startplasma-x11</code></td>
</tr>
<tr>
<td style="text-align:right"><code>lxde</code></td>
<td style="text-align:center">Light weight X11</td>
<td><code>startlxde</code></td>
</tr>
<tr>
<td style="text-align:right"><code>xfce4 xfce4-goodies</code></td>
<td style="text-align:center">X Forms Common</td>
<td><code>startxfce4</code></td>
</tr>
</tbody>
</table>
</details>

  ```bash
  sudo apt install -y `DESKTOP` 
  ```

+ **Setting Virtual Network Computing ( VNC ) Server**
  ```bash
  PWDx=$PWD && cd $HOME && rm -rf VNC && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx
  ```
+ **cammand for start or stop vnc**
  ```bash
  vnc 
  ```
<h2 align=center>
  N joy !
</h>

<h5 align=right>Bonus 🥳</h5>

```bash
sudo apt install -y firefox fonts-indic fonts-emojione openjdk-8-jdk

# Mozilla
# Indian Fonts - हिंदी, देवनागरी, मराठी, ગુજરાતી, ਪੰਜਾਬੀ, ಕನ್ನಡ, മലയാളം, తెలుగు, … etc, etc.
# Emojies - 😎, 😃, ❤, 😍, 😂, 👍, 😊, 🎉 … etc, etc.
# java, javac, appletviewer, jar … etc, etc.
```

[SS](Simple.md)

+ Install TermUX opener on Ubuntu
  ```bash
  wget https://raw.githubusercontent.com/ShivaShirsath/Ubuntu-On-Android/main/TermUX.desktop -O $HOME/Desktop/TermUX.desktop && chmod +x $HOME/Desktop/TermUX.desktop
  ```
