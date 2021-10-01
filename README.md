# File Share Platform

This acts as a master repository for deploying the file share platform.

## Simple Production Deployment

```sh
git clone https://github.com/file-share-platform/file-share-platform 
cd file-share-platform

cp .example.env .env
nano .env # Update domain and email for letsencrypt config, set a long random database password

docker-compose --env-file .env up
```