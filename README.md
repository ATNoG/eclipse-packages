# Eclipse IoT Packages™ [![Gitter chat](https://badges.gitter.im/eclipse/packages.png)](https://gitter.im/eclipse/packages)

IoT Packages is an effort by the [Eclipse IoT working group](https://iot.eclipse.org/), to create easy to deploy Eclipse IoT based, end-to-end scenarios, on top of Kubernetes and Helm.

See: https://eclipse.org/packages

## Submodules

This repository contains submodules for each of the packages. To clone the repository with all submodules, use:

```bash
git clone git@github.com:ATNoG/eclipse-packages.git
cd eclipse-packages
git checkout atnog-packages
git submodule update --init --recursive
```

## Package Charts

### Ditto

```bash
helm dependency update charts/ditto/deployment/helm/ditto
helm package charts/ditto/deployment/helm/ditto
```

### Hono

```bash
helm dependency update charts/hono
helm package charts/hono
```

### Cloud2Edge

```bash
helm dependency update packages/cloud2edge
helm package packages/cloud2edge
```
