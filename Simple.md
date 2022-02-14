+ **TermUX Level**
  ```bash
  pkg update -y && pkg upgrade -y && pkg install proot-distro -y && proot-distro install ubuntu && proot-distro login ubuntu
  ```
+ **CLI Level**
  ```bash
  apt update -y && apt upgrade -y && apt install sudo -y && sudo apt update -y && sudo apt upgrade -y && sudo apt install dialog && adduser shiva && echo "shiva ALL=(ALL:ALL) ALL" >> /etc/sudoers && echo "proot-distro login --user shiva ubuntu" >> $PREFIX/bin/ubuntu && chmod +x $PREFIX/bin/ubuntu && login shiva
  ```
+ **GUI Level**

<!--
  ```bash
  sudo apt install -y xfce4 xfce4-goodies git firefox fonts-indic fonts-emojione openjdk-8-jdk && PWDx=$PWD && cd $HOME && rm -rf VNC && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx
  ```
-->
+ **Login to ubuntu**
  ```bash
  ubuntu
  ```
+ **Logout**
  ```json
  exit # Or [ Ctrl+d ]
  ```
+ **Desktop**
  ```bash
  vnc
  ```
