# vamp-spike
Trying out VAMP with some JAX-RS like service routing.

## Start vamp
    docker run --net=host \
               -v /var/run/docker.sock:/var/run/docker.sock \
               -v $(which docker):/bin/docker \
               -v "/sys/fs/cgroup:/sys/fs/cgroup" \
               -e "DOCKER_HOST_IP=localhost" \
               magneticio/vamp-docker:0.8.2-marathon
