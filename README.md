# Riptide

This acts as a master repository for deploying Riptide.

## Development Setup

```sh
git clone git@github.com:riptide-org/riptide.git --recursive
cd riptide

cp .example.dev.env .dev.env
nano .dev.env # Update port etc if you'd like

./dev.sh
```

## Simple Production Deployment

```sh
git clone git@github.com:riptide-org/riptide.git --recursive
cd riptide

cp .example.env .env
nano .env # Update APP_HOST

docker-compose up
```
