# What are containers and how are they different?

![container architecture](/docker-fundamentals/00_LearningAids/DOCKER101-ContainerArchitecture.png)

<a href = "https://aws.amazon.com/compare/the-difference-between-containers-and-virtual-machines/#:~:text=application%20is%20deployed.-,Key%20differences%3A%20containers%20vs.,use%20your%20hardware%20resources%20efficiently.">Containers vs VMs</a>

<a href = "https://aws.amazon.com/compare/the-difference-between-docker-vm/">Docker vs. VM</a>

## Virtual Machine Drawback

-  Running multiple guest operating systems consumes a lot of resources, especially when it comes with duplicate operating systems.

## Container Architecture

- Docker container engine is lighter than a hypervsior because it has less to do.

- Any container on this Docker host shares the same host OS - they run as a process on the OS. 

- Containers do not need to run their own individual OS. They only need to run the libraries, runtime environment, and application. This makes containers more light weight and efficient.

- On physical hardware, running containers instead of VMs = more free capacity.

## Container Architecture Summary

- Containers run on a container host

- .. via container (Docker) Engine

- Containers only run an APP & libraries/Runtime Environment

- Share the container HOST OS (run as a process on it)

- Lightweight - Can be densely packed & started/restarted quickly

- Can be impacted by other continaers (noisy neighbors)

- Containers are designed to hold an application, as well as everything that application needs to function. Example: A developer created an application on his own machine, but when it came time to ship it, the app did not work. Develop and run on container to keep dependencies consistent.