# README

### Environment Variables

| Variable | Description | Where to Obtain |
| --- | --- | --- |
| PASSWORD | Server password | Create a new server user and set the password.

### Container Description

This Docker Compose file sets up a Valheim server, allowing you to play with friends.

### Quick Start Guide

1. Update the `PASSWORD` environment variable with your actual server password.
2. Run `docker-compose up -d` to start the container.
3. Access the Valheim dashboard at <http://your-domain-name:2456>.

### Extra Information

* Make sure to update the `PASSWORD` environment variable with your actual user password.
* If you encounter any issues, refer to the [Valheim documentation](https://www.valheim-game.com/documentation/server/).
