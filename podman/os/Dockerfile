FROM quay.io/fedora/fedora-bootc:40

RUN dnf groupinstall -y --nobest --excludepkgs rootfiles "KDE Plasma Workspaces"

RUN systemctl enable sddm \
&& systemctl set-default graphical.target 

RUN dnf install -y podman podman-compose distrobox \ 
&& systemctl enable podman