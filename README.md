Docker Tutorials

Best youtube channel : https://www.youtube.com/channel/UC0NErq0RhP51iXx64ZmyVfg : Name : - 
Bret Fisher Docker and DevOps

## Major Docker ways to run containers
- Locally (Docker Desktop, RD)
- Server (Docker Engine, K8s)
- PaaS (Cloud Run, Fargate)

## Local container runtimes in 2024, tools for running containers for local dev

## Resources\Local container runtimes in 2024, tools for running containers for local dev - Sheet1.csv

## Docker command format
* new command way --> docker <command> <sub-command> (options)
* old command way --> docker <command> (options) [STILL WORKS]

## Image vs Container
* Defination : A Docker image is a lightweight, standalone, executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, environment variables, and configurations. It is built from a Dockerfile, which specifies the environment and steps needed to create the image.

* Key characteristics of Docker images include:
1. Immutable: Once built, a Docker image is read-only and cannot be changed. Any changes to the image result in the creation of a new image.

2. Layered: Docker images are composed of multiple layers. Each layer represents a set of changes made to the image, such as adding files, installing software, or modifying configurations.

3. Portable: Docker images can be easily shared and distributed. They contain all dependencies needed to run the application, ensuring consistency across different environments.

4. Versioned: Docker images can be versioned using tags (e.g., nginx:latest, nginx:1.21). This allows for easy tracking and retrieval of specific versions of software.

5. Efficient: Docker uses a Union File System to optimize storage and minimize redundancy between images and layers. This means that when multiple images or containers share the same base image or layers, they only need to store the differences.

6. Buildable: Docker images are built using Dockerfiles, which are text files that specify the instructions to assemble the image. This makes it easy to automate the build process and ensure reproducibility.

#### Docker images are fundamental to Docker containers, which are lightweight, portable, and self-sufficient execution environments that can run on any Docker-compatible system, whether it's a developer's laptop, a data center VM, or a cloud instance. Containers are instantiated from Docker images and provide a consistent environment for running applications and services, regardless of the underlying infrastructure.
* An Image is the application we want to run
* A container is an instance of that image running as a process
* We can have many containers running of the same image
* Docker's default image "registry" is called Docker Hub (hub.docker.com)

### Docker commands and their Descriptions
1. docker version --> verified cli can talk to engine
2. docker info --> most config values of engine
3. docker container --help --> Get the list of commands