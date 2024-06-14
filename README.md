# rnd-bpnt-directus
Render Blueprint - Directus

Uses the `directus/directus:10` Docker image, and the latest version of PostgreSQL supported by Render's Database Service. Requires several Environment Variables to be set in the Render Dashboard.

Creates two resources on Render:

- Database - `ab-directus-db`
- Web Service - `ab-directus-server`