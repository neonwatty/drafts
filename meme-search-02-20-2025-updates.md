


# Meme search updates 02-20-2025

Quality of life updates to the Pro version of Meme Search, including:

- bugfixes in the image-to-text service that makes cancelling failed jobs more reliable
- new custom ports / hosts options to more easily run the pro app with tools like Unraid and Portainer, or if you need to run its services on different ports / hosts
- new local build compose file for building and testing locally `docker-compose-pro-local-build.yml`
- new `grid view` in both home and search pages for a broader view of your memes (see animation below)

<p align="center">
<img align="center" src="https://github.com/jermwatt/readme_gifs/blob/main/meme-search-grid-view-medium.webp" height="225">
</p>


- you can now [customize hosts names and ports](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#custom-hosts-and-ports) for easier usage with NAS, Portainer, Unraid, or if you just need to customize! 
- 4 new image to text new models added ranging in size from 200M to 2B parameters: florence-2-base (new default), florence-2-large, smolvlm-256, smolvlm-500
- new model selection panel added in the pro app Settings so you select or change your image-to-text model
- moondream2 to current revision
- new test database added to image-to-text service for more comprehensive testing
- new [local docker compose files added](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#building-the-app-locally-with-docker) for easier local building and testing
- gh action test and build scripts refactored for easier (local) testing
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MjMxMzE0OTNdfQ==
-->