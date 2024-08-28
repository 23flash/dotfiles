FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper ar -f https://download.opensuse.org/repositories/devel:/tools:/ide:/vscode/openSUSE_Tumbleweed devel_tools_ide_vscode \
&& zypper --gpg-auto-import-keys ref \
&& zypper in -y --no-recommends code