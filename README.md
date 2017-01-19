# Docker Compose stack for Homie Dashboard

This repository contains pre-built Docker images for easy bootstrapping of 
Homie Dashboard.

## Features

* AMD64 and ARMhf support
* Mosquitto embedded
* TLS-secured

## Installation

* Install Git, Docker and Docker Compose
* Clone this repository:
```bash
git clone https://github.com/INTECH-RGB/homie-dashboard-docker-compose.git
```
* `cd homie-dashboard-docker-compose`
* Tweak the configuration file at [./homie-dashboard/settings.toml](homie-dashboard/settings.toml)
* Add your `cert.pem` and `key.pem` files in [./caddy](caddy/)
* Run the stack:
```bash
# Replace `armhf` with `amd64` if needed
# If no ARCH is provided, `amd64` is used by default
ARCH=armhf docker-compose up -d
```
