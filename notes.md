Notes: 
## What is docker?
- used for building, running, and shipping apps in a consistent manner
- used to package all dependencies of an app in a consistent manner
- app packaged in container, virtual environment with all dependencies contained within

## Virtual machines vs Containers
- container: an isolated environment for running an application
- virtual machine (VM): an abstraction of a machine (physical hardware)
- Problems with VMS
  - needs a full-blown OS
  - slow to start
  - resource intensive
- Benefits of containers:
  - allow running mutliple apps in isolation
  - lightweight
  - use OS of the host
  - starts quickly
  - less resource intensive

## Docker Architecture
- Client/Server architecture communicating via REST API
  - Server known as docker engine
  - Containers are processes on docker engine
  - all containers share the kernel of the host (kernel manages applications and hardware resources)
  - each OS has different kernel with different APIs, so containers can only run in their respective OS 
    - Linux only run Linux containers
    - Windows can run both Windows and Linux Containers
    - Mac OS uses Linux VM