# Getting Started
## Requirements
* Kubernetes Cluster
* Helm Installed

## Helm Installation
To start, you need to install the helm repository. This can be done via:
```bash
helm repo add fallernetes https://mirrorstudios.github.io/fallernetes-helm
```

### Application Configuration
Next, if you wish to see and edit the values, you can do:
```bash
helm show values fallernetes/fallernetes > output.yaml
```
This prints the default values to `output.yaml`, where you can edit them.

### Application Installation
To install the application with default values, run:
```bash
helm install fallernetes fallernetes/fallernetes 
```

If you need to use a specific files value, add `-f fileName.yaml`, so:
```bash
helm install fallernetes fallernetes/fallernetes -f fileName.yaml
```

Once the application is installed, you can create a simple Server as discussed in [Server](server.md).