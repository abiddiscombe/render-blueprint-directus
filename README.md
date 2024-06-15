# Render Blueprint - Directus

An example [Render Blueprint](https://docs.render.com/infrastructure-as-code) (Render's IaC Product) for configuring and deploying a [Directus](https://directus.io/) instance, backed by [PostgreSQL](https://www.postgresql.org/). Feel to use this template for your own projects; make sure to apply any customisations you require such as modifying a resource's `region` and `name` values.

## Resources

By default, these resources are deployed in the *Frankfurt* region on a *Starter* plan.

### Web Service - 🐇

The `directus-server` web service deploys the `directus/directus:10` Docker image, with administrative credentials defined via the Render Dashboard during the initial sync. The `10` tag uses the `10.x.x` major version whilst recieving bug fixes and new features.

### PostgreSQL Database - 🐘

The `directus-db` database uses the latest version of PostgreSQL supported by Render, with all external IPs (non-Render connections) blocked.