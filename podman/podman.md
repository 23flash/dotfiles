[`home`](https://github.com/23flash/dotfiles)

`how to build dockerfiles with podman`
```bash
podman build -t "imagenamehere" -f Dockerfile
```
`how to run  podman container `

```bash
podman run --name "containername" "imagenamehere"
```
`how to run kasm test Enviroment`
```bash
podman run --rm -it --shm-size=512m -p 6901:6901 -e VNC_PW=password "imagenamehere"
```
- Standart Login
   - User : kasm_user
   - Password: password
