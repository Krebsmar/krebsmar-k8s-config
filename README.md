# krebsmar-k8s-config

This repository contains a set of cloud native services as blueprint for Kubernetes Cluster operations. This configuration have my personall touch and reflacting my current state of knowledge. This configurations are for non productive use and just support hands-on sessions.

### Before you begin

- You know Linux
- You know Kubernetes
- You know Version Control with Git, best on Github

## Kind Cluster

For a local environment you can use [Kind](https://kind.sigs.k8s.io/). In ./kind you will find a basic Kind config to setup a cluster with control-plane and 3 workers.

```
cd ./kind
```

```
kind create cluster --name mycluster --config ./kind-config.yaml
```

## Version Control
- I'm using Github
- Create Repository
- Create Personal Access Token with permissions to work on repositories

## Install Flux CLI

```
curl -s https://fluxcd.io/install.sh | sudo bash
```

## Export your Credentials

```
export GITHUB_TOKEN=<your-token>
export GITHUB_USER=<your-username>
```