# Theia Kubernetes

Theia is a cloud & desktop IDE framework implemented in TypeScript. http://theia-ide.org

Basic Authentication default user/password is `user`/`P@ssw0rd`.  
You can overwrite user/password by environment variables.(`USER`/`PASSWORD`)

## How to use `theia-kubernetes` image?

### local

This script pulls the image and runs Theia IDE on http://localhost:3000 with the current directory as a workspace.
```
docker run -it -p 3000:3000 -v "$(pwd):/home/project:cached" gashirar/theia-kubernetes:latest
```

### k8s cluster

Apply yaml!
```
kubectl apply -f theia.yaml
```
