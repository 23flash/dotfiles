FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper in -y --no-recommends vim git btop mc duf wget curl fd rsync openssh fish eza

RUN zypper ar -f \
      https://download.opensuse.org/repositories/Virtualization:/Appliances:/Builder/openSUSE_Tumbleweed/ \
      kiwi-appliance-builder \
&& zypper --gpg-auto-import-keys ref \
&& zypper in -y --no-recommends python3-kiwi