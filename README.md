# dotfiles
My Personal Dotfiles

# Distrobox
includes Distrobox images and ini files for distrobox assemble
# Github Workflows
to automate image building

# Podman 
## how to build dockerfiles with podman
- podman build -t "imagenamehere" -f Dockerfile

## how to run  podman container 
podman run --name "containername" "imagenamehere"

## how to run kasm test Enviroment 
podman run --rm -it --shm-size=512m -p 6901:6901 -e VNC_PW=password "imagenamehere"
- Login
    - User : kasm_user
    - Password: password