```bash
docker network ls
# to inspect a network
docker network inspect bridge
# connect a container to a network
docker network connect my-net my-container
# dis connect from a network
docker network disconnect my-net my-container
# remove a specific network
docker network rm network-name
# remove unused network
docker network prune
# create a network
docker network create --driver=bridge --subnet=193.168.10.0/24 network-name
```

It is possible to connect a container to multiple network
embeded dns does not work with default bridge network