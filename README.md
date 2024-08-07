# Quickstart Quarkus and Postgres on Minikube

## Installation

Install podman
```bash
brew install podman
````

Install podman desktop (optional)
```bash
brew install podman-desktop
```

Install Minikube:
```bash
brew install minikube
```

Install Quarkus CLI
```bash
brew install quarkusio/tap/quarkus
```

Start Minikube with :
```bash
minikube start --driver=podman
```

Start the dashboard if you like:
```bash
minikube dashboard
```

## Developer Mode

Build and start the application in developer mode
```bash
quarkus dev
```

## Minikube

### Build
```bash
quarkus build
```

### Deploy
```bash
quarkus deploy
```

### Run

Check port of kubus services:
```bash
kubectl get serivices
```

```bash
minikube service kubus
```

Adjust port of the kubusservice:
```bash
curl http://127.0.0.1:<PORT>/fruit
```
