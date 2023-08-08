# About TopoMojo

TopoMojo -- _Topo_ for short -- is a web application used for creating and delivering cybersecurity training labs and exercises. With TopoMojo, users can build and deploy labs in a highly-isolated and secure virtual-machine environment.

TopoMojo allows for the same functionality and connectivity that users would experience with real, physical devices. Network topologies can utilize not only IP and Ethernet, but also custom protocol solutions, like 802.11 wireless packet simulation.

New topologies can be rapidly deployed using existing templates or built from the ground up with user-provided ISO's and VM specifications.

This documentation introduces users to the TopoMojo environment and provides information necessary to launch existing labs and create new topologies.

**Go to the TopoMojo repository:** [github.com/cmu-sei/TopoMojo](https://github.com/cmu-sei/TopoMojo)

## Topo concepts

You build your content in a *workspace*; but you "play" (complete the lab, do the activity) in a *gamespace*. The workspace is where a virtual topology is built. Here, engineers and lab developers add VMs, save updates, author a guide in Markdown, and configure questions/answers to turn the topology into a lab or *challenge*. 

A *gamespace* is where someone else plays through the lab. They get their own, isolated, read-only copies of all workspace resources. Players in a gamespace can interact with VMs and answer questions to complete a lab, but they can't save anything in the environment. 

In short: a *gamespace* is a read-only copy of a *workspace* where a player (user) interacts with the lab content.

The term *challenge* refers to when both Gameboard and TopoMojo are integrated to execute a cyber competition. In this scenario, Gameboard is a consumer of content made in TopoMojo. More information on that is available elsewhere in the Foundry documentation.