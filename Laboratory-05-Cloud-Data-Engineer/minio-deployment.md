# MinIO Deployment Documentation

## 1. Deployment Overview

For Mission 5: The Cloud Data Engineer, I deployed an S3-compatible object storage server using Docker in a KillerCoda Ubuntu Playground. The original `minio/minio` image specified in the laboratory instructions could not be downloaded, so I used the alternative `pgsty/minio` image. The container started successfully and provided access to the Silo web console.

## 2. Docker Command Used

The following is the exact command I used to deploy the server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
pgsty/minio server /data --console-address ":9001"
```

## 3. Port Configuration

- **Port 9000:** Used for the object storage API.
- **Port 9001:** Used to access the web console through KillerCoda's port-access feature.

The Docker `-p` flags map the container ports to the corresponding ports on the playground environment.

## 4. Bucket Created

- **Bucket name:** `client-photos`
- **Access setting:** Private
- **Uploaded test file:** `sample.txt`

The bucket stores uploaded objects and provides a separate location for the sample file used to verify the storage operation.

## 5. Environment Variables

The `-e` flags in the Docker command set environment variables inside the container.

- `MINIO_ROOT_USER=cloudadmin` sets the administrator username.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password.

These variables configure the credentials used to log in to the storage console.

## 6. Verification

I verified the deployment using `docker ps`, which showed that the `minio-server` container was running and that ports 9000 and 9001 were mapped. I also checked the container logs and successfully accessed the Silo console. Finally, I created the `client-photos` bucket and uploaded `sample.txt`.

## 7. Deployment Note

The laboratory PDF specifies the `minio/minio` image. Because Docker could not download that image in my environment, I used `pgsty/minio` instead. This difference is documented to accurately reflect the commands and configuration used during the activity.
