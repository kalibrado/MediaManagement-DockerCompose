# Docker Compose for Media Management

 Effortlessly organize and access your digital content with this comprehensive configuration.


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
- **Jellyseerr:** is a free and open source software application for managing requests for your media library. It is a a fork of Overseerr built to bring support for Jellyfin & Emby media servers!
- **Jellyfin** is a Free Software Media System that puts you in control of managing and streaming your media. It is an alternative to the proprietary Emby and Plex, to provide media from a dedicated server to end-user devices via multiple apps.

## Setup and Configuration

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/kalibrado/MediaManagement-DockerCompose.git
    cd MediaManagement-DockerCompose/
    ```

2. **Set Environment Variables:**
    - Adjust environment variables in a `.env` file for PUID, PGID, TZ, DOCKER_MODS, HOST, PORTS, PATH_CONFIG, PATH_DOWNLOADS, and PATH_DATA.

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
    - `http://[HOST]:[PORT_JELLYSEER]`
    - `http://[HOST]:[PORT_JELLYFIN]`

- **FlareSolverr:** Configure as needed and integrate with other services.

## Or use portainer 

- Create new stack 
  ![image](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/d85e39d3-6f5b-4d0e-b420-57f4bd5fa695)
- Paste docker composer file content
  ![image](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/62dec701-a50f-4a72-9d69-4a4359be086a)
- Edit and paste .env file 
  ![image](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/e6bc5ef7-e755-4ab6-8b8c-0469548e1870)
- Deploy stack 
  ![image](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/6b49602a-a82c-4c87-8f6c-c36d21466e21)
- Enjoy!!
  ![image](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/da294ef1-2ec2-48d8-8f74-e0092588a16f)
 



## Additional Notes

- **Dependencies:** Services are interconnected, and dependencies are managed automatically.

- **Volumes:** Data and configuration files are stored in specified volumes for persistence.

- **Customization:** Adjust paths and settings to suit your preferences and system configuration.

This Docker Compose configuration streamlines the deployment of media management tools, making it easy to manage and organize your digital media effortlessly.

![Annotation 2024-01-15 104845](https://github.com/kalibrado/MediaManagement-DockerCompose/assets/51781584/20957419-67e4-4339-8ee2-c2f2cea4422a)

## Sources

https://github.com/FlareSolverr/FlareSolverr

https://wiki.servarr.com/

https://docs.linuxserver.io/

https://docs.theme-park.dev/themes

https://github.com/Fallenbagel/jellyseerr

https://jellyfin.org/docs/

[!["Buy Me A Beer"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/leonardofod)
