FROM dorowu/ubuntu-desktop-lxde-vnc

RUN apt-get update

RUN apt-get install ssh -y

RUN apt-get install unzip -y

run apt-get clean

RUN service ssh start 

EXPOSE 22

COPY id_rsa.pub .

RUN mkdir -p  /root/.ssh/authorized_keys && cp id_rsa.pub /root/.ssh/authorized_keys



