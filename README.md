# Islandora CLAW: Blazegraph Docker Image

[![Docker Stars](https://img.shields.io/docker/stars/islandora/claw-blazegraph.svg)](https://hub.docker.com/r/islandora/claw-blazegraph/)
[![Docker Pulls](https://img.shields.io/docker/pulls/islandora/claw-blazegraph.svg)](https://hub.docker.com/r/islandora/claw-blazegraph/)

## Introduction

Defines the Blazegraph Docker image. 

Based on the [Tomcat Docker Image](https://github.com/Islandora-CLAW/docker-tomcat).

## Includes

* Blazegraph

## Build Arguments

| Variable           | Required | Default |
|--------------------|----------|---------|
| BLAZEGRAPH_VERSION | no       |   1.5.1 |

**Example:**
```bash
docker build -t islandora/claw-blazegraph .
```

## Environment Variables

No additional environment variables provided.

Please consult the [parent image](https://github.com/Islandora-CLAW/docker-tomcat).

**Example (foreground, port 8080, auto-remove):**
```bash
docker run --rm -ti -p 8080:8080 -e "TOMCAT_ADMIN_PASSWORD=your_super_secure_password" islandora/claw-blazegraph
```

## Commands

For convenience a number of commands are provided in the [commands](/commands) folder.

| Command    | Arguments               | Defaults    | Notes                                                            |
|------------|-------------------------|-------------|------------------------------------------------------------------|
| build      |                         |             | Build this image with the default settings.                      |
| foreground | [port] [admin password] | 8080 random | Start tomcat in the foreground with the given port and password. |
| background | [port] [admin password] | 8080 random | Start tomcat in the background with the given port and password. |

## Maintainers/Sponsors

* UPEI
* discoverygarden inc.
* LYRASIS
* McMaster University
* University of Limerick
* York University
* University of Manitoba
* Simon Fraser University
* PALS
* American Philosophical Society
* common media inc.

Current maintainers:

* [Nigel Banks](https://github.com/nigelgbanks)
* [Nick Ruest](https://github.com/ruebot)

## Development

If you would like to contribute, please get involved by attending our weekly [Tech Call](https://github.com/Islandora-CLAW/CLAW/wiki). We love to hear from you!

If you would like to contribute code to the project, you need to be covered by an Islandora Foundation [Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_cla.pdf) or [Corporate Contributor Licencse Agreement](http://islandora.ca/sites/default/files/islandora_ccla.pdf). Please see the [Contributors](http://islandora.ca/resources/contributors) pages on Islandora.ca for more information.

## License

[MIT](https://opensource.org/licenses/MIT)
