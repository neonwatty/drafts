


# Meme Search v 1.1.5 release notes

updated 02-20-2025

Major updates and quality of life improvements, image to text model additions,  UX upgrades made to the Pro version of the app including:

**Quality of life updates:**
- 10x reduction in Docker image size for app / image-to-text services
- Easier custom setup of the Pro App for local NAS, Portainer, Unraid, etc., 
with newly enabled [customize hosts names and ports](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#custom-hosts-and-ports) 
- new smaller (200M - 10x smaller than previous) cutting edge default image to text model for faster local processing on most machines


**New image to text models:**

- 4 new cutting edge [image to text new models](https://github.com/neonwatty/meme-search?tab=readme-ov-file#features---pro-version) added ranging in size from 200M to 2B parameters
- moondream2 updated to version 2.0

**UX improvements:**
- new model selection panel added in the Pro app Settings so you select or change your image-to-text model at will (illustrated below)

<p align="center">
<img align="center" src="https://github.com/jermwatt/readme_gifs/blob/main/meme-search-model-selection-screen-demo.webp" height="225">
</p>

- new `grid view` both home and search pages for a broader view of your memes (illustrated below)

<p align="center">
<img align="center" src="https://github.com/jermwatt/readme_gifs/blob/main/meme-search-grid-view-medium.webp" height="225">
</p>

**Improved local builds and testing:**

- new local build compose file for building and testing locally `docker-compose-pro-local-build.yml`
- new test database added to image-to-text service for more comprehensive testing
- new [local docker compose files added](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#building-the-app-locally-with-docker) for easier local building and testing
- gh action test and build scripts refactored for easier (local) testing


See the [README.md](https://github.com/neonwatty/meme-search/blob/main/README.md) and [CHANGELOG.md](https://github.com/neonwatty/meme-search/blob/main/CHANGELOG.md) for further details on updates and bugfixes.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM5ODAxNTg2OCwxNjEzNjM1MTIwLDE5Mj
Y4OTA5MTZdfQ==
-->