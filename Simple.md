+ **TermUX Level**
  ```bash
  apt update -y && apt upgrade -y && apt install proot-distro -y && proot-distro install ubuntu && PWDx=$PWD && cd $HOME && rm -rf VNC && apt install -y git && git clone https://github.com/ShivaShirsath/VNC.git && cd VNC && bash install && cd $PWDx && proot-distro login ubuntu
  ```
+ **CLI Level**
  ```bash
  clear && apt update -y && apt upgrade -y && apt install -y sudo && sudo apt update -y && sudo apt upgrade -y && sudo apt install -y dialog && read -p $'\e[1;31m[\e[0m\e[1;93m●\e[0m\e[1;31m]\e[0m\e[1;92m User Name \e[1;91m[ \e[1;93mlower case \e[1;91m]\e[1;92m :\e[0m\e[1;96m\en' user && echo -e "${W}" && echo "$user ALL=(ALL:ALL) ALL" >> /etc/sudoers && adduser $user && echo "proot-distro login --user $user ubuntu" > /data/data/com.termux/files/usr/bin/ubuntu && chmod +x /data/data/com.termux/files/usr/bin/ubuntu && login $user
  ```
+ **GUI Level**

  ```bash
  cd ~ && sudo apt install -y wget git && rm -rf set && wget https://raw.githubusercontent.com/ShivaShirsath/Ubuntu-On-Android/main/set && chmod +x set && bash set
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
