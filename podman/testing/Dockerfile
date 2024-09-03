FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper in -y --no-recommends zsh curl git
RUN sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" --unattended
