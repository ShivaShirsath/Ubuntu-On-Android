+ **TermUX Level**
  ```bash
  pkg update -y && pkg upgrade -y && pkg install proot-distro -y && proot-distro install ubuntu && PWDx=$PWD && cd $HOME && rm -rf VNC && apt install -y git && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx && proot-distro login ubuntu
  ```
+ **CLI Level**
  ```bash
  apt update -y && apt upgrade -y && apt install -y sudo && sudo apt update -y && sudo apt upgrade -y && sudo apt install -y dialog && adduser shiva && echo "shiva ALL=(ALL:ALL) ALL" >> /etc/sudoers && echo "proot-distro login --user shiva ubuntu" >> /data/data/com.termux/files/usr/bin/ubuntu && chmod +x /data/data/com.termux/files/usr/bin/ubuntu && login shiva
  ```
+ **GUI Level**

  ```bash
  cd ~ && apt install -y wget git && rm -rf set && wget https://raw.githubusercontent.com/ShivaShirsath/Ubuntu-On-Android/main/set && chmod +x set && bash set
  ```

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
