FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper in -y --no-recommends vim git btop mc duf wget curl fd rsync openssh fish eza

RUN zypper ar -f https://download.opensuse.org/repositories/editors/openSUSE_Tumbleweed/editors.repo \
&& zypper --gpg-auto-import-keys ref \
&& zypper in -y --no-recommends zed


RUN zypper ar -f https://download.opensuse.org/repositories/devel:/tools:/ide:/vscode/openSUSE_Tumbleweed devel_tools_ide_vscode \
&& zypper --gpg-auto-import-keys ref \
&& zypper in -y --no-recommends code