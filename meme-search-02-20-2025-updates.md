


# Meme Search v 1.1.5 release notes

updated 02-20-2025

Major updates and quality of life improvements made to the Pro version of the app including:

**New models:**
- 10x reduction in Docker image size
- Easier custom setup of the Pro App for local NAS, Portainer, Unraid, etc., 
with [customize hosts names and ports](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#custom-hosts-and-ports) 
- 4 new cutting edge image to text new models added ranging in size from 200M to 2B parameters
- new smaller (200M) cutting edge default image to text model for faster local processing on most machines
- - moondream2 update to current revision

**Quality of life improvements:**
- new model selection panel added in the Pro app Settings so you select or change your image-to-text model at will (

<p align="center">
<img align="center" src="https://github.com/jermwatt/readme_gifs/blob/main/meme-search-model-selection-screen-demo.webp" height="225">
</p>


- new `grid view` in both home and search pages for a broader view of your memes (see animation below)

<p align="center">
<img align="center" src="https://github.com/jermwatt/readme_gifs/blob/main/meme-search-grid-view-medium.webp" height="225">
</p>

- bugfixes in the image-to-text service that makes cancelling failed jobs more reliable

**Improved local builds and testing:**

- new local build compose file for building and testing locally `docker-compose-pro-local-build.yml`
- new test database added to image-to-text service for more comprehensive testing
- new [local docker compose files added](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#building-the-app-locally-with-docker) for easier local building and testing
- gh action test and build scripts refactored for easier (local) testing



See the [README.md](https://github.com/neonwatty/meme-search/blob/main/README.md) and [CHANGELOG.md](https://github.com/neonwatty/meme-search/blob/main/CHANGELOG.md) for additional updates and bugfixes.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3MzQyNjM1MzcsMTkyNjg5MDkxNl19
-->