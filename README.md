# Kompose project

This repository contains a basic example of using the Kompose tool to convert a Docker Compose file into Kubernetes manifests.
## what is kompose?

## Installation 
1- **First, you need to download the Kompose** :
```bash
wget https://github.com/kubernetes/kompose/releases/download/v1.24.0/kompose-linux-amd64
```
2- **Make the binary executable** : 
```bash
chmod +x kompose-linux-amd64
```
3- **Move the binary to a directory in your PATH** :
```bash
sudo mv kompose-linux-amd64 /usr/local/bin/kompose
```
4- **Verify the installation**:
```bash
 kompose version
```
## Usage
After installing the Kompose tool, you need to have a `docker-compose.yml` file. Here, we have a file to set up a Nextcloud application. By running the command the Docker Compose file will be converted into the necessary manifest files for running it on a Kubernetes platform.
```bash
 kompose convert --file docker-compose.yml
```

