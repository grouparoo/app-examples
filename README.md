# Grouparoo App Examples

All the repositories linked here are automatically kept up-to-date with the latest releases of Grouparoo.

## Configuration Examples

> Examples configuring Grouparoo via [Declarative Sync](https://www.grouparoo.com/docs/config).

### [`grouparoo/app-example-config`](https://github.com/grouparoo/app-example-config)

Connects a database with `users` and `purchases` to create properties. Creates a few groups from that data related to high value users. Syncs data with Mailchimp.

### [`grouparoo/app-example-csv`](https://github.com/grouparoo/app-example-csv)

Connects to a remote CSV file to import Grouparoo profile data.

### [`grouparoo/app-example-snowflake-salesforce`](https://github.com/grouparoo/app-example-snowflake-salesforce)

Use Grouparoo to connect Snowflake to Salesforce.

## Integration Examples

> Examples of using working with other platforms.

### [`grouparoo/app-example-dbt`](https://github.com/grouparoo/app-example-dbt)

Shows how to use Grouparoo within a [dbt](https://www.getdbt.com) project to sync data to destinations after using dbt to do the transformations.

## Deployment Platform Examples

> Before you deploy, it's important to understand [Grouparoo's deployment topology](https://www.grouparoo.com/docs/support/network), [environment variables](https://www.grouparoo.com/docs/support/environment), and [how to secure your Grouparoo cluster](https://www.grouparoo.com/docs/support/security).

### [`grouparoo/app-example-cloud`](https://github.com/grouparoo/app-example-cloud)

An example application deployed on Grouparoo Cloud, with configuration validation on pull requests and automatic deployment on merge to `main`.

### [`grouparoo/app-example-heroku`](https://github.com/grouparoo/app-example-heroku)

An example application ready to deploy Grouparoo to Heroku. This repository also includes the code for the "Deploy to Heroku" Button.

### [`grouparoo/app-example-aws`](https://github.com/grouparoo/app-example-aws)

An example application ready to deploy Grouparoo to Amazon Web Services (AWS) via Elastic Beanstalk & CodeDeploy.

### [`grouparoo/app-example-gcp`](https://github.com/grouparoo/app-example-gcp)

An example application ready to deploy Grouparoo to Google Cloud Platform (GCP) via node.js.

### [`grouparoo/app-example-docker`](https://github.com/grouparoo/app-example-docker)

This repository shares how to build your own Docker images for Grouparoo, and how to deploy it with either Docker Compose or Kubernetes.
