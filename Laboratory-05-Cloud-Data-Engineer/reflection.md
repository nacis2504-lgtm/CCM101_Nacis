# Mission Reflection

This laboratory helped me understand why cloud object storage is useful for managing a large amount of data. Object storage is better suited for storing millions of photos because it is designed to handle large numbers of individual files as objects. Unlike traditional block storage, object storage can organize data using buckets and metadata, making it easier to manage and access many files. It can also be scaled when the amount of stored data increases.

Using Docker made the deployment of MinIO easier because I did not have to manually install and configure every required component. With a Docker command, the MinIO server could be started inside a container with the required ports and environment variables. This made the setup process more organized and easier to repeat if the server needed to be deployed again.

A bucket is a storage container used to organize objects in cloud storage. In this laboratory, the bucket named `client-photos` was used to store sample files. It works like a main folder where related objects can be placed and managed.

Large enterprise companies can protect their object storage data by using multiple copies of data, redundancy, backups, and replication across different servers or locations. If one physical server fails, another copy of the data can still be available. They may also use monitoring systems and recovery procedures to detect failures and restore services.

My confidence in using the Linux command line is also improving. At first, I was not very familiar with Docker and Linux commands, so I had to carefully follow each step. After running commands, checking container status, and troubleshooting errors, I became more comfortable working in the terminal. This laboratory showed me that learning through hands-on practice makes command-line tasks easier to understand.
```

