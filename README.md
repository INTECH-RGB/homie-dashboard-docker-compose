# Docker Compose stack for Homie Dashboard

This repository contains pre-built Docker images for easy bootstrapping of 
Homie Dashboard.

## Features

* AMD64 and ARMhf support
* Mosquitto embedded

## Installation

* Install Git, Docker and Docker Compose
* Clone this repository:
```bash
git clone https://github.com/INTECH-RGB/homie-dashboard-docker-compose.git
```
* `cd homie-dashboard-docker-compose`
* Tweak the configuration file at [homie-dashboard/settings.toml](homie-dashboard/settings.toml)
* Run the stack:
```bash
# Change `amd64` by `armhf` if needed
docker-compose -f docker-compose.yml -f amd64.yml up -d
```
