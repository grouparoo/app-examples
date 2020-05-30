# Grouparoo app-example

![Node.js CI](https://github.com/grouparoo/app-example/workflows/Node.js%20CI/badge.svg)

An example Grouparoo deployment. This project includes:

- An example `package.json` for using Grouparoo
- An example `Procfile` for Heroku-like deployments
- An example `Dockerfile` for building a docker image from this project, along with a `docker-compose.yml` for linking Grouparoo to associated services (Redis and Postgres), and splitting work between web and worker nodes.
- Example Kubernetes files to deploy this application to AWS EKS

Learn more at https://github.com/grouparoo/grouparoo/blob/master/documents/deployment

I am built automatically to https://hub.docker.com/r/grouparoo/app-example yielding the `grouparoo/app-example` docker image.
I am tested automatically via Github Actions against multiple versions of node.js.
