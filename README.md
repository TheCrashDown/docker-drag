# Docker pull python script (Google mirror, works in Russia)

This is a fork of NotGlop/docker-drag script, adapted to be used with Google Cloud mirror (mirror.gcr.io).   

As a result, this implementation can work from Russia and another countries, blocked by Docker Hub. 

## Purpose

Pull images from Docker Hub without having Docker installed on your machine.  

## Usage example

```
pip install requests

python docker_pull.py python:3.12-slim
```

After the image has been downloaded (`.tar` file), you can then import it and use it with the following docker commands:

```
docker load -i library_python.tar
docker image list
```
