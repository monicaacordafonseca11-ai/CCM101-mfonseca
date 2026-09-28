# Cloud Storage Types Research

## Comparison Table

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splits data into fixed-size blocks, each with a unique identifier. Functions like an unformatted physical hard drive attached to a server. | High-performance databases, operating system boot volumes, transactional systems. | Amazon EBS (Elastic Block Store) |
| **File Storage** | Hierarchical file system structure with folders and subfolders. Accessible via standard network protocols like NFS or SMB/CIFS. | Shared network drives, central file repositories, legacy application file sharing. | Amazon EFS (Elastic File System) |
| **Object Storage** | Stores data as discrete objects containing raw data, customizable metadata, and a unique global ID within a flat address space. | Massive unstructured data storage, media hosting, backups, static websites. | Amazon S3 (Simple Storage Service) |

---

## Client Recommendation

Object Storage is the ideal choice for storing user-uploaded images because web application containers are ephemeral (temporary) and cannot safely store persistent data[span_15](start_span)[span_15](end_span). Object Storage provides a flat namespace with unlimited horizontal scalability and direct HTTP/HTTPS access, eliminating the performance and cost bottlenecks of traditional file or block systems when handling millions of media files[span_16](start_span)[span_16](end_span).
Laboratory-05-Cloud-Data-Engineer/storage-types-research.md
