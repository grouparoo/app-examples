# Grouparoo Helm Chart

## Generating

The files in this directory are generated from `docker-compose.published.yml` with the `kompose` tool - https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/. The images used in these examples will be using the [`grouparoo/app-example` docker image](https://hub.docker.com/repository/docker/grouparoo/app-example). This image is built automatically from the master branch of this repository. _You should not run this image in production_ - rather you should build your own image with only the Grouparoo plugins you wish to use.

To regenerate the kubernetes/helm files in this repository, run the tool `./bin/generate-helm`, which relies on the `kompose` tool already being installed

## Running

Ensure that you have both docker and Kubernetes running locally. If you are using Docker Desktop, you can do this from the Prefrences pane:

> TODO: IMAGE

You can run the generated Helm Chart locally with the helm command - https://helm.sh/docs/intro/install/

Assuming you have Docker and Kubernetes running locally: `cd helm && helm install grouparoo-app-example . --replace`
