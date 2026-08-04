# README

### Environment Variables

| Variable | Description | Where to Obtain |
| --- | --- | --- |
| DB_PASSWORD | Database password | Create a new database user and set the password.
| MYSQL_ROOT_PASSWORD | MySQL root password | Create a new MySQL root user and set the password.

### Container Description

This is a Docker Compose file for running BookLore, an online cataloging application. It includes two services: BookLore and MariaDB.

### Quick Start Guide

1. Update the `DB_PASSWORD` environment variable with your actual database password.
2. Update the `MYSQL_ROOT_PASSWORD` environment variable with your actual MySQL root user password.
3. Run in portainer.
4. Access the BookLore dashboard at <http://your-domain-name:6060>.

### Extra Information

* Make sure to update the `DB_PASSWORD` and `MYSQL_ROOT_PASSWORD` environment variables with your actual passwords.
* If you encounter any issues, refer to the [BookLore documentation](https://booklore-app.github.io/booklore/docs/).
