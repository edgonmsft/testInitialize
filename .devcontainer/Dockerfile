FROM ubuntu:latest

ARG USERNAME=codespace
ARG USER_UID=1000
ARG USER_GID=$USER_UID
ARG HOMEDIR=/home/$USERNAME

RUN apt-get update
RUN useradd -s /bin/bash --uid $USER_UID -m $USERNAME
#RUN echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME
#RUN chmod 0440 /etc/sudoers.d/$USERNAME
RUN mkdir -p /home/$USERNAME
