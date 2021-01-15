# Docker

## Docker Build

```bash
# Build Image from current working directory
docker build .

# Build Image with tag
docker build -t railsapp -t railsapp:1.0
```

## Docker Images

```bash
# List Images in System
docker images

# Remove image
docker rmi image_name_or_id
docker image rm image_id
```

## Docker Run

```bash
# Run image with default configured command
docker run -p 3000:3000 railsapp

# Run Rails server command in container created from specified image ID
docker run -p 3000:3000 1a69f7e73251 bin/rails s -b 0.0.0.0

# Run rails server command in container created from specified image tag
docker run -p 3000:3000 railsapp bin/rails s -b 0.0.0.0
```

## Docker Tag

```bash
# Tag image with custom name
docker tag 1a69f7e73251 railsapp
```
