# beszel/docker-compose.yaml Readme
=====================================

## Overview

This is a `docker-compose` file for the Beszel application.

### Services

* `beszel`: The main Beszel service. It uses the `henrygd/beszel` image and exposes port 9090 on the host machine.
* `/beszel_data`: A volume that maps to the `beszel_data` directory in the current working directory.

## Configuration

* `APP_URL`: Sets the URL of the application to http://localhost:8090
* `restart`: The container will restart unless it is explicitly stopped.

### Volumes

* `./beszel_data:/beszel_data`: Maps the `beszel_data` directory in the current working directory to a volume within the container.