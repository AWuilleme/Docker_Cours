ARG SYSTEM_LINUX=ubuntu:latest
FROM ${SYSTEM_LINUX}

RUN apt-get update && \
apt-get upgrade -y && \
apt-get install -y \
net-tools \
sudo \
openjdk-17-jdk -y \
unzip \
wget \
screen -y \
iputils-ping -y \
nano -y \
ufw -y 
 
RUN cd home && \
wget https://github.com/AWuilleme/Docker_Cours/raw/main/minecraft.zip && \
unzip minecraft.zip && \
rm minecraft.zip && \
cd minecraft && \
wget https://launcher.mojang.com/v1/objects/125e5adf40c659fd3bce3e66e67a16bb49ecc1b9/server.jar && \
chmod +x start.sh && \
ufw allow 25565




