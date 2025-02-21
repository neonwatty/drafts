


> Written with [StackEdit](https://stackedit.io/).The open source engine indexes your memes by their visual content and text, making them easily searchable. Drag and drop recovered memes into any messager.


Thanks to community feedback, we're excited to release a major update, featuring quality-of-life improvements, image-to-text models, UX enhancements, and local build/test upgrades!   [original post](https://www.reddit.com/r/selfhosted/comments/1e3x6l0/i_built_a_free_open_source_locally_hosted_search/) 

These updates include:

**Quality of life updates:**
- 4 new cutting edge [image to text new models](https://github.com/neonwatty/meme-search?tab=readme-ov-file#features---pro-version)  ranging in size from 200M to 2B parameters cutting edge default image-to-text model added for faster local processing on most machines
- 4 new cutting edge added 
- 
- 10x reduction in Docker image size for app services
- Easier custom setup of the for local NAS, Portainer, Unraid, etc., 
use with newly enabled [customize hosts names and ports](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#custom-hosts-and-ports) 

**New image to text models:**


- moondream2 updated to version 2.0

**UX improvements:**
- new model selection panel added in Settings allowing for choice of image-to-text model at will
- new `grid view` added to both home and search pages for a broader view of your memes


**Improved local builds and testing:**

- new local build compose file for building and testing locally `docker-compose-pro-local-build.yml`
- new test database added to image-to-text service for more comprehensive testing
- new [local docker compose files added](https://github.com/neonwatty/meme-search/tree/main?tab=readme-ov-file#building-the-app-locally-with-docker) for easier local building and testing
- gh action test and build scripts refactored for easier (local) testing
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAzMzg1Mjk2Ml19
-->