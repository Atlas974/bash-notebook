# jupyter/bash-notebook
Based on : https://raw.githubusercontent.com/jupyter/docker-stacks/master/datascience-notebook/Dockerfile

## Build
Run `docker build -t bash-notebook .`.  

## Use
Run `docker run --rm -p 8888:8888 -v "${PWD}:/root" bash-notebook`.  
All the files you save while working in the container are written to the host (`--rm` removes the container when closing).
