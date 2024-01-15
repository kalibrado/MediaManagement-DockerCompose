# Docker Compose for Media Management
Docker Compose Suite for Media Management: Streamline the deployment and automation of your media management tools, including Prowlarr, Sonarr, Lidarr, Radarr, Readarr, Lazylibrarian, Mylar3, and FlareSolverr. Effortlessly organize and access your digital content with this comprehensive configuration.




## Overview

This Docker Compose file simplifies the deployment of various media management tools, providing a comprehensive solution for organizing and automating your digital content. It includes the following services:

- **Prowlarr:** Indexer manager/proxy supporting both Torrent Trackers and Usenet Indexers.
- **Sonarr:** PVR for usenet and bittorrent users, focusing on TV shows.
- **Lidarr:** Music collection manager for Usenet and BitTorrent users.
- **Radarr:** Movie manager, a fork of Sonarr tailored for movies.
- **Readarr:** Book manager and automation, akin to Sonarr but for ebooks.
- **Lazylibrarian:** Program to follow authors and grab metadata for digital reading needs.
- **Mylar3:** Automated Comic Book downloader supporting NZB, torrents, and more.
- **FlareSolverr:** Proxy server to bypass Cloudflare and DDoS-GUARD protection.

## Setup and Configuration

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/kalibrado/MediaManagement-DockerCompose.git
    cd MediaManagement-DockerCompose/
    ```

2. **Set Environment Variables:**
    - Define environment variables in a `.env` file (create if not present) for PUID, PGID, TZ, DOCKER_MODS, HOST, PORTS, PATH_CONFIG, PATH_DOWNLOADS, and PATH_DATA.

3. **Configure Services:**
    - Adjust configuration settings for each service in the `docker-compose.yml` file.

4. **Run Docker Compose:**
    ```bash
    docker-compose up -d
    ```

5. **Access Services:**
    - Each service can be accessed via the specified ports on your host machine.

## Usage

- **Prowlarr:** Visit `http://[HOST]:[PORT_PROWLARR]` for indexer management and integration with other PVR apps.

- **Sonarr, Lidarr, Radarr, Readarr, Lazylibrarian, Mylar3:**

    Access respective services via
    - `http://[HOST]:[PORT_SONARR]`
    - `http://[HOST]:[PORT_LIDARR]`
    - `http://[HOST]:[PORT_RADARR]`
    - `http://[HOST]:[PORT_READAR]`
    - `http://[HOST]:[PORT_LAZYLIBRARIAN]`
    - `http://[HOST]:[PORT_MYLAR3]`

- **FlareSolverr:** Configure as needed and integrate with other services.

## Additional Notes

- **Dependencies:** Services are interconnected, and dependencies are managed automatically.

- **Volumes:** Data and configuration files are stored in specified volumes for persistence.

- **Customization:** Adjust paths and settings to suit your preferences and system configuration.

This Docker Compose configuration streamlines the deployment of media management tools, making it easy to manage and organize your digital media effortlessly.
