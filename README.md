<h1 align=center> Ubuntu On Android </h1>

# ![dark](https://user-images.githubusercontent.com/59221352/158588323-e051658f-a71f-47f6-bd19-0fe984c97e28.jpg)
# ![light](https://user-images.githubusercontent.com/59221352/158586852-1c1fec70-3698-44e3-82ce-a884008540c9.jpg)

**TermUX → [Download](https://f-droid.org/packages/com.termux) /
[Install](https://play.google.com/store/apps/details?id=com.termux)**

+ **Install [Proot-Distro](https://github.com/termux/proot-distro) & Ubuntu CLI & Login to CLI**

```bash
pkg update -y && pkg upgrade -y && termux-setup-storage && pkg install -y proot-distro git && proot-distro install ubuntu && echo "proot-distro login ubuntu" > /data/data/com.termux/files/usr/bin/ubuntu && chmod +x /data/data/com.termux/files/usr/bin/ubuntu && PWDx=$PWD && cd $HOME && rm -rf VNC && apt install -y git && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx && ubuntu
```

+ **Ubuntu GUI ( xfce4 )**

```bash
cd ~ && sudo apt install -y wget dialog git && rm -rf set && wget https://raw.githubusercontent.com/ShivaShirsath/Ubuntu-On-Android/main/set && chmod +x set && sudo bash set
```

+ **Login**
  ```bash
  ubuntu
  ```
+ **Logout**
  ```json
  exit
  ```
  ```json
  [ Ctrl+d ]
  ```
+ **Desktop**
  ```bash
  vnc
  ```

<!--
+ Add User
```bash
adduser <UserName> && echo "<UserName> ALL=(ALL:ALL) ALL" >> /etc/sudoers
```
+ **Install udisks2**
```bash
rm -rf /var/lib/dpkg/info/*.postinst && sudo dpkg --configure -a && sudo apt install udisks2 -y && rm -rf /var/lib/dpkg/info/*.postinst && sudo dpkg --configure -a
```
-->
<p align=center><a href=Simple.md>ss</a></p>
