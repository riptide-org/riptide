# File Share Platform

This acts as a master repository for deploying the file share platform.

## Development Setup

```sh
git clone https://github.com/file-share-platform/file-share-platform --recursive
cd file-share-platform

cp .example.dev.env .env
nano .env # Update port and host if desired

docker-compose -f docker-compose.dev.yml --env-file .env up
```

## Simple Production Deployment

```sh
git clone https://github.com/file-share-platform/file-share-platform --recursive
cd file-share-platform

cp .example.env .env
nano .env # Update domain and email for letsencrypt config, set a long random database password

docker-compose --env-file .env up
```