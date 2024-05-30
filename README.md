# docker-drag (Google mirror, work in Russia)

This is a fork of NotGlop/docker-drag script, adapted to be used with Google docker mirror.   

This implementation can work from Russia and another countries, banned by Docker Hub. 

## Usage example

`python docker_pull.py python:3.12-slim`

After the image has been downloaded (`.tar` file), you can then import it and use it with the following docker commands:

```
docker load -i library_python.tar
docker run -it python
```