Introduction
---

This is a work in progress. This repository tries to deploy the GDI starter-kit stack in one place. 

* The starter-kit repositories are added as submodules of this repository. Use ```git clone --recurse-submodules ...``` to clone this repository with the submodules.
* [docker-compose.yml](docker-compose.yml) includes each submodule docker-compose and a corresponding ```override.yml```. These overrides contain all the modification that has to be performed to deploy the full stack. Use simply ```docker compose up``` to deploy the full stack.
* Extra configuration files are added in the configuration folder. Because the extra files are added to mounted volumes, Macos requires changing the following `Settings > General > Virtual Machine Options > file sharing implementation > gRPC FUSE`

Diagram
---
Diagram representing the components of the stack. It can be modified with the `Draw.io Integration` extension in VS-Code.

![diagram.drawio.svg](diagram.drawio.svg)