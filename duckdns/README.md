# README

### Environment Variables

| Variable | Description | Where to Obtain |
| --- | --- | --- |
| SUBDOMAINS | Comma-separated list of subdomains | List your subdomains, separated by commas (e.g. `sub1,sub2,sub3`) 
| YOUR_DUCKDNS_TOKEN | Duck DNS token | Create a new Duck DNS account and generate an API token

### Container Description

Duck DNS is a cloud-based Dynamic DNS service.
This container automatically updates your Duck DNS record, allowing you to access your device remotely using a custom domain.

### Quick Start Guide

1. Replace the `SUBDOMAINS` environment variable in the `docker-compose.yml` file with your desired subdomain (e.g. `example.duckdns.org`).
2. Replace the `YOUR_DUCKDNS_TOKEN` environment variable in the `docker-compose.yml` file with your actual Duck DNS API token.
3. Run in portainer
4. Log on to your Duck DNS account and create a new DNS entry for your subdomain.
5. Access your device remotely using your custom domain (e.g. `http://example.duckdns.org:80`).

### Extra Information

* Make sure to update the `SUBDOMAINS` environment variable with your actual subdomains, separated by commas.
* If you encounter any issues, refer to the [Duck DNS documentation](https://duckdns.org/documentation.html).
