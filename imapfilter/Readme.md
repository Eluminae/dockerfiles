# Image

Docker image of ArchLinux with imapfilter installed.

# Usage

Just bind mount your config into /home/imapfilter/.imapfilter/config.lua and run your container !

```bash
vim config.lua
```

```yaml
# docker-compose.yml
version: '3'

services:
  imapfilter:
    image: eluminae/imapfilter
    volumes:
      - config.lua:/home/imapfilter/.imapfilter/config.lua
```
