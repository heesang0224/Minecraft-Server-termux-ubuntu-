# Minecraft-Server-termux-ubuntu-
안드로이드 스마트폰앱 termux에 우분투를 설치하고 마인크래프트 서버를 실행하는법

---
##Contents
1. termux, anLinux Download
2. termux settings
3. termius download and settings
4. java installation
5. server start

---
##Download
1. termux download - <https://f-droid.org/ko/packages/com.termux/>
2. anLinux download - <https://f-droid.org/ko/packages/exa.lnx.a/>

---
##Settings
Ubuntu installation

    pkg update
    pkg upgrade

anLinux ubuntu select -> copy -> termux paste

---
##ubuntu start

    ./start-ubuntu.sh
    apt update
    apt install openssh-server -y
    service ssh start
    hostname -I
    passwd

---
##ssh setting

edit

Port 8022

PermitRootLogin yes

PasswordAuthentication yes

    mkdir -p /run/sshd
    service ssh restart

---
##in termius 
1. new host
2. address (your server ip)
3. port --> 8022
4. username --> root
5. password --> your password
🧨connect
    
    
---
##java

    apt install openjdk-25-jdk

---
##server start

create server file

    mkdir [server name]
    cd [server name]

---
##downloads paper
<https://papermc.io/>


    wget -O paper.jar [Paper 다운로드 URL]

---
##server start


    java -Xms4G -Xmx4G -jar paper.jar nogui


eula=true










    






    
