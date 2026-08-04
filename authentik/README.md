# README

### Environment Variables

| Variable | Description | Where to Obtain |
| --- | --- | --- |
| POSTGRES_PASSWORD | PostgreSQL password | Create a new PostgreSQL user and set the password.
| AUTHENTIK_SECRET_KEY | Authentik secret key | Generate a random secret key, you can use a tool like [Faker](https://faker.readthedocs.io/en/master/)
| AUTHENTIK_HOST | Authentik host | Set this to your domain name (e.g. `auth-zhang-server-pc.duckdns.org`)
| AUTHENTIC_DOMAIN | Authentic domain | Set this to the same value as `AUTHENTIK_HOST`

### Container Description

Authentik is an open-source identity and access management platform.

### Dependencies

* Install Docker and Docker Compose on your system.

### Quick Start Guide

1. Update the `traefik.http.routers.authentik.rule` label in the `docker-compose.yml` file to match your domain name.
2. Update the `volumes` section in the `docker-compose.yml` file to reference your NAS storage (e.g. `/srv/storage/NAS/docker-meta/authentik/`).
3. Run in portainer
4. Access the Authentik dashboard at <http://your-domain-name:9000> or <https://{{AUTHENTIC_DOMAIN}}>.

### Extra Information

* Make sure to update the `traefik.http.routers.authentik.rule` label with your actual domain name.
* If you encounter any issues, refer to the [Authentik documentation](https://authentik.io/docs/).