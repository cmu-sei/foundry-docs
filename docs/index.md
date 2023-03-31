# Welcome to Foundry Docs

!!! warning ""

    :construction: This site is under construction. Stay tuned for more updates. :construction:

Welcome to the home of *Foundry Docs*. The documentation describes how to deploy, configure, and use the Foundry application stack developed by the [Software Engineering Institute](https://www.sei.cmu.edu) (SEI) at [Carnegie Mellon University](https://www.cmu.edu). The Foundry app stack consists of **Identity**, **TopoMojo**, and **Gameboard**. **Foundry Appliance** is also documented here. Identity plus TopoMojo plus Gameboard equals a full cyber competition and training environment.

## Identity

Identity manages authentication with OpenID Connect (OIDC) and OAuth 2.0.

- **Repo:** [github.com/cmu-sei/identity](https://github.com/cmu-sei/identity)
- **Identity doc:** [Identity Guide](identity/index.md)

## TopoMojo

TopoMojo is virtual lab builder and player. Create training content and publish it so other people can consume it.

- **Repo:** [github.com/cmu-sei/topomojo](https://github.com/cmu-sei/topomojo)
- **TopoMojo doc:** [TopoMojo Guide](topomojo/index.md)

## Gameboard

Gameboard is a web platform that provides game design capabilities and a competition-ready user interface.

- **Repo:** [github.com/cmu-sei/Gameboard](https://github.com/cmu-sei/Gameboard)
- **Gameboard doc:** [Gameboard Guide](gameboard/index.md)

## Appliance

Foundry Appliance is a virtual machine that integrates Identity, TopoMojo, and Gameboard. It's built using Ubuntu and [Lightweight Kubernetes](https://k3s.io/) (K3s).

- **Repo:** [github.com/cmu-sei/foundry-appliance](https://github.com/cmu-sei/foundry-appliance)
- **Foundry Appliance doc:** [Appliance Guide](appliance/index.md)