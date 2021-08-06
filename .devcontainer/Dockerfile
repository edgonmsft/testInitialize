FROM ubuntu:latest

ARG USERNAME=codespace
ARG USER_UID=1000
ARG HOMEDIR=/home/$USERNAME

RUN apt-get update
RUN useradd -s /bin/bash --uid $USER_UID -m $USERNAME
RUN mkdir -p /home/$USERNAME
RUN mkdir -p /etc/sudoers.d
RUN echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME
