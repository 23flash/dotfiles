FROM quay.io/toolbx/arch-toolbox:latest as base

RUN pacman -Syu --noconfirm git base-devel sudo

RUN echo "Defaults         lecture = never" > /etc/sudoers.d/privacy \
 && echo "%wheel ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/wheel \
 && useradd -m -G wheel -s /bin/bash builder


USER builder
WORKDIR /aur

RUN git clone https://aur.archlinux.org/yay.git \
  && cd yay \
  && makepkg -sri --needed --noconfirm \
  && cd \
  && rm -rf .cache yay
