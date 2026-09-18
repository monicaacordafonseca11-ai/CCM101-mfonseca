# Laboratory 04: The Cloud-Native Engineer

## Mission Overview
This laboratory explores containerization fundamentals using Docker, shifting away from full virtual machine abstractions to deploy scalable, lightweight services.

## Objectives
* Differentiate between traditional Virtual Machines (VMs) and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate a containerized application (Nginx).
* Create technical documentation using Markdown within GitHub.

## Docker Commands Executed
* `docker --version`: Checks installed Docker version.
* `docker info`: Displays system-wide Docker status and details.
* `docker pull nginx`: Downloads Nginx image from Docker Hub.
* `docker run -d -p 8080:80 --name my-nginx nginx`: Runs Nginx in detached mode on port 8080.
* `curl http://localhost:8080`: Tests web server accessibility via terminal.
* `docker ps`: Displays running containers.
* `docker stop my-nginx`: Stops execution of the target container.
* `docker ps -a`: Lists all containers including stopped ones.
* `docker rm my-nginx`: Removes the stopped container instance.

## Skills Learned
* Port forwarding and networking configurations between host systems and isolated containers.
* Management of basic container lifecycles via CLI tooling.
* Comparative understanding of operating-system-level virtualization vs. hardware-level virtualization.

## Challenges Encountered
* Managing port bindings ensuring external requests map correctly to the container's isolated web port.
