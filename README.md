# Quick Start Guide

This repo has the compose files to host things on a home lab

You will need docker server to be installed on the server pc.

## 1 - Decisions to be made early
- The linux distro to use
- You NAS
- Registering a Domain

## 2 - NAS Decision
You can buy a Synology to run the nas or you can use Samba 
to network share.

## 3 - Domain/DNS
You can buy a domain and register it through cloudflare.
The 'free' option is to use duck dns which is what this stack uses.
[See DuckDNS Docs here](duckdns/README.md)

## 4 - VPN
You have several options like OpenVpn. This stack uses Netbird which comes with a reverse proxy built in. The set up is different than just a simple compose script so read the documentation [here](https://docs.netbird.io/selfhosted/selfhosted-quickstart). Make sure to set this up outside of portainer.


## Portainer
This is what this stack uses to manage all docker containers. Make sure to deploy all containers using this instead of using the `docker compose up` in the console.

***This needs to be the first thing that gets deployed***

To deploy a new service go to `stacks -> new stack -> web -> copy and past yaml`. Make sure to update the env variables.
## Readme Files

Here are some links to other Readme files:
* [Valheim Server](valheim/README.md)
* [Portainer](portainer/README.md)
* [Pi-hole](pi-hole/README.md)
* [Minecraft Server](minecraft-server/README.md)
* [Minecraft Bedrock Server](minecraft-bedrock-server/README.md)
* [DuckDNS](duckdns/README.md)
* [Booklore](booklore/README.md)
* [Authentik](authentik/README.md)


