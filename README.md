# Docker image with [SageMath](http://www.sagemath.org/) + [JupyterHub](https://jupyterhub.readthedocs.io/)

For use with [DockerSpawner](https://github.com/jupyterhub/dockerspawner).

## Dependencies

Your Hub must be running JupyterHub 0.8

## Install

    docker pull defeo/jupyterhub_sagemath:latest

## Configure the Hub

In your `jupyterhub_config.py`, set

```python
c.JupyterHub.spawner_class = 'dockerspawner.DockerSpawner'
```

and

```python
c.DockerSpawner.image = 'paulbrou/jupyterhub_sagemath:latest'
```
