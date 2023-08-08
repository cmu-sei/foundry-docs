# Getting started

## Installing

Installing Topo is a matter of installing the Helm chart found [here](https://github.com/cmu-sei/helm-charts/tree/main/charts/topomojo) on the SEI's GitHub page. The CMU-SEI Helm charts repo is a public repository on GitHub for anyone to access and use. The Topo chart contains two sub-charts: `topomojo-api` and `topomojo-ui`. The `api` and the `ui` are different apps and need to be deployed separately.

!!! info

    This structure is consistent with the other Foundry apps: there is an `api` piece and a `ui` piece.

**TopoMojo values.yaml:** Contains default configurations for the `api` and the `ui`. To deploy TopoMojo, configure the **Values.yaml** file according to your needs and `helm install` TopoMojo.

## What's new

Get the latest Topo source code and its accompanying release notes [here](github.com/cmu-sei/TopoMojo/releases).