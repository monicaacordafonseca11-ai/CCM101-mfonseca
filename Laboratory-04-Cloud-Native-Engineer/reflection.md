# Mission Reflection

Provisioning a traditional Virtual Machine requires instantiating an entire operating system kernel, virtual hardware allocations, and full system boot sequences, taking several minutes. In contrast, Docker containers share the host operating system's kernel while isolating processes through Linux namespaces and cgroups. This lightweight architecture allows containers to launch almost instantaneously (seconds or milliseconds) while consuming significantly less system memory.

Port mapping (`-p 8080:80`) is necessary because containers reside in private, isolated network namespaces by default. The Nginx web server listens on internal port 80 inside its container; mapping it to host port 8080 bridges external host traffic directly to the isolated service.

Executing `docker rm` permanently destroys the container instance and its writable filesystem layer. Any unpersisted data created inside the container during runtime is lost unless attached to persistent storage volumes.

Containerization fundamentally shifts DevOps workflows by standardizing software deployment packages. Developers and operations teams can package applications along with dependencies into identical container images, eliminating environment discrepancies ("it works on my machine") and speeding up deployment pipelines across multi-cloud infrastructure.

My GitHub portfolio is expanding to demonstrate modern cloud-native capabilities alongside traditional cloud infrastructure modeling.
