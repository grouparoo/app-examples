# Grouparoo app-example

![Node.js CI](https://github.com/grouparoo/app-example/workflows/Node.js%20CI/badge.svg)

I am an example Grouparoo deployment. This project includes:

- An example `package.json` for using Grouparoo and a few common plugins.
- An example `Procfile` for Heroku-like deployments.
- An example `Dockerfile` for building a docker image from this project, along with a `docker-compose.yml` for linking Grouparoo to associated services (Redis and Postgres), and splitting work between web and worker nodes.
- Example Kubernetes files to deploy this application to AWS EKS.

Learn more at https://www.grouparoo.com/docs/deployment

I am built automatically to https://hub.docker.com/r/grouparoo/app-example yielding the `grouparoo/app-example` docker image.
I am tested automatically via Github Actions against multiple versions of node.js.

### Deploy to Heroku

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/grouparoo/app-example)

### Run locally with Docker & Docker Compose

Assuming you have Docker installed:

```bash
# in a new directory
curl -L https://www.grouparoo.com/docker-compose --output docker-compose.yml
docker-compose up
```

### To run me locally:

1. Clone this repo (`git clone https://github.com/grouparoo/app-example.git`)
2. Ensure that you have node.js (v12+), Redis, and Postgres installed locally
3. `cp .env.example .env` and check that those values work for your local setup
4. `npm install`
5. `npm start`

Grouparoo releases stable versions against the `latest` npm tag, but also releases weekly against the `next` npm tag. To try the newest versions of grouparoo (our "Beta" builds), change "latest" to "next" within the `package.json`, and then run `npm install` again. You can learn more about the [Grouparoo release process here](https://github.com/grouparoo/grouparoo/blob/master/documents/development/publishing.md).

## Having Trouble?

If you are having trouble, visit the list of [common issues](https://www.grouparoo.com/docs/deployment/common-issues) or open a [Github issue](https://www.grouparoo.com/support) to get support.
