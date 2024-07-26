*The notes here are sourced from this video: https://www.youtube.com/watch?v=fqMOX6JJhGo*

## DOCKER RUN

### RUN - Tags
```
docker run redis
```
VS
```
docker run redis:4.0
```
### RUN - Stdin
Normally, docker ignores any requests for input. We can fix this by adding `-t` and `-i` as options to the `run` command.