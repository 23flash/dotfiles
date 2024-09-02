FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper ar -f https://download.opensuse.org/repositories/editors/openSUSE_Tumbleweed/editors.repo \
&& zypper --gpg-auto-import-keys ref \
&& zypper in -y --no-recommends zed
