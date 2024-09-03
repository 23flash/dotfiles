FROM registry.opensuse.org/opensuse/distrobox:latest

RUN zypper in -y --no-recommends vim git btop mc duf wget curl fd rsync openssh zsh eza
RUN wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh || true
