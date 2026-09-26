# MinIO Server Deployment


This documentation presents the steps performed to deploy a MinIO object storage server using Docker. It also covers the Web Console access, bucket creation, file upload, and the environment variables used during deployment.

---

## 1. Deploying MinIO with Docker

The MinIO server was launched using the following Docker command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

### Docker Command Details

| Option | Purpose |
|---|---|
| `docker run` | Creates and starts the MinIO container. |
| `-d` | Keeps the container running in the background. |
| `-p 9000:9000` | Connects host port 9000 to the MinIO service port 9000. |
| `-p 9001:9001` | Connects host port 9001 to the MinIO Web Console port. |
| `--name minio-server` | Assigns `minio-server` as the container name. |
| `-e "MINIO_ROOT_USER=cloudadmin"` | Defines `cloudadmin` as the root administrator username. |
| `-e "MINIO_ROOT_PASSWORD=CloudNova2026!"` | Defines the root administrator password. |
| `minio/minio` | Identifies the MinIO image used by Docker. |
| `server /data` | Starts MinIO with `/data` as its storage location. |
| `--console-address ":9001"` | Sets port 9001 as the Web Console address. |

---

## 2. Opening the MinIO Console

After starting the container, the MinIO Web Console was opened through **port 9001**.

In the KillerCoda Playground, port `9001` was entered under **Traffic / Ports** or **Custom Ports**, and the **Access** option was selected.

### Console Port

```text
9001
```

The two ports used by the deployment are:

- **9000** - MinIO API and storage service
- **9001** - MinIO Web Console

---

## 3. Logging In to MinIO

The administrator credentials specified in the Docker command were used to access the MinIO Web Console.

**Username:**

```text
cloudadmin
```

**Password:**

```text
CloudNova2026!
```

These credentials were configured through the MinIO environment variables.

---

## 4. Creating the Storage Bucket

After entering the MinIO Web Console, the **Buckets** menu was selected.

A new bucket was created using the following name:

```text
client-photos
```

The bucket was then opened to manage its stored objects.

---

## 5. Adding a Sample File

The **Upload** option inside the `client-photos` bucket was used to add a test file.

The file uploaded was:

```text
sample.txt
```

The successful appearance of `sample.txt` inside the bucket confirmed that the MinIO storage service was able to accept and store objects.

---

## 6. Environment Variables

The `-e` option in Docker is used to pass **environment variables** to the container. In this deployment, the variables were used to configure the MinIO administrator account.

### Root Username

```bash
-e "MINIO_ROOT_USER=cloudadmin"
```

This variable specifies the username of the MinIO root administrator.

The configured username is:

```text
cloudadmin
```

### Root Password

```bash
-e "MINIO_ROOT_PASSWORD=CloudNova2026!"
```

This variable specifies the password associated with the MinIO root administrator account.

The username and password are used when signing in to the MinIO Web Console.

---

## 7. Deployment Configuration

| Configuration | Value |
|---|---|
| Application | MinIO |
| Container | `minio-server` |
| Docker Image | `minio/minio` |
| Storage Directory | `/data` |
| API Port | `9000` |
| Console Port | `9001` |
| Administrator Username | `cloudadmin` |
| Bucket | `client-photos` |
| Test File | `sample.txt` |

---

## 8. Result

The MinIO object storage server was deployed successfully through Docker.

The Web Console was made available through port `9001`, and the administrator account was used to access the interface. The `client-photos` bucket was created successfully, and `sample.txt` was uploaded as a test object.

The completed deployment demonstrated that the MinIO server was operational and capable of storing files through its Web Console.

---

