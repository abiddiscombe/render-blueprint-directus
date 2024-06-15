# Render Blueprint - Directus

An example [Render Blueprint](https://docs.render.com/infrastructure-as-code) (Render's IaC Product) for configuring and deploying a [Directus](https://directus.io/) instance, backed by [PostgreSQL](https://www.postgresql.org/).

Feel free to repurpose this template for your own use: copy the `render.yaml` file into a new **private** repository and apply any customisations such as modifying the resource's `region` and `name` values.

## Resources

By default, the following resources are deployed in the *Frankfurt* region on a *Starter* plan.

### Web Service - 🐇

The `directus-server` web service deploys the `directus/directus:10` Docker image, with administrative credentials defined via the Render Dashboard during the initial sync.

### PostgreSQL Database - 🐘

The `directus-db` database uses the latest version of PostgreSQL supported by Render, with all external IPs (non-Render connections) blocked.