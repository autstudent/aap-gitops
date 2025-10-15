# Openshift Cluster Bootstrap

This Helm chart tries to collect the different Openshift objects to bootstrap the cluster.

## Introduction

*Openshift Cluster Bootstrap* chart deploys the following elements:

- Operator Subscriptions

## Install

- Install Helm Chart

```$bash
helm install bootstrap . 
```

- Install Helm Chart applying objects in kubernetes

```$bash
helm template . --debug | oc apply -f -
```

## Local Tests

- Lint

```$bash
helm lint
```

- Dry run installations

```$bash
helm install bootstrap . --dry-run --debug
```

- Render templates Locally

```$bash
helm template . --debug
```

## Author Information

Asier Cidon @RedHat
