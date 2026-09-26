# Cloud Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Stores data in individual blocks that can be accessed separately. It functions like a virtual hard drive and provides fast and direct access to stored data. | Best for operating systems, databases, virtual machines, and applications that need high-performance storage. | **AWS EBS (Elastic Block Store)** |
| **File Storage** | Stores data as files arranged in folders and directories. It uses a traditional file system that makes files easy to organize, access, and share. | Best for shared files, documents, media, and applications that require a traditional file system. | **AWS EFS (Elastic File System)** |
| **Object Storage** | Stores data as objects along with metadata and a unique identifier. These objects are organized inside containers called buckets for easier management and access. | Best for storing large amounts of unstructured data such as images, videos, documents, and backups. | **AWS S3 (Simple Storage Service)** |

## Why Object Storage is the Best Choice

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It organizes the images into buckets, making them easier to store, access, and manage as the application grows to millions of photos.
