# Repull all Docker Hub images

One-liner to repull all Docker Hub images. Replace `podman` with `docker` if you use `docker`:

```bash
podman images --format '{{.Repository}}:{{.Tag}}' 'docker*/*/*' | xargs -L1 podman pull
```
