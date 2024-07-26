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
### RUN - Port Mapping
Every docker container is assigned an internal IP address and port, so the docker host can access the container using: 
```
http://[internal IP]:[internal port]
```
But what about external devices? We can use the IP of the docker host instead by mapping the internal port on the container to a free port on the local host. Like this: 
```
docker run -p [local port]:[internal port] somedockercontainer
```
where the user would connect like 
```
http://[host IP]:[mapped local port]
```