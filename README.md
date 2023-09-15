# Shrinking-Docker-image

This guide will walk you through the process of building the smallest possible Docker image. By following these steps, you'll achieve a more than 1000x reduction in image size compared to the initial one.

**Dockerfile.big**  
docker build -t go-big -f Dockerfile.big .  
docker image ls go-big  
docker run -ti --rm go-big  

**Dockerfile.alpine**  
docker build -t go-alpine -f Dockerfile.alpine .  
docker image ls go-alpine  
docker run -ti --rm go-alpine  

**Dockerfile.multi-stage**  
docker build -t go-multi-stage -f Dockerfile.multi-stage .  
docker image ls go-multi-stage  
docker run -ti --rm go-multi-stage  

**Dockerfile.scratch**  
docker build -t go-scratch -f Dockerfile.scratch .  
docker image ls go-scratch  
docker run -ti --rm go-scratch  

**Dockerfile.stripped**  
docker build -t go-stripped -f Dockerfile.stripped .  
docker image ls go-stripped  
docker run -ti --rm go-stripped  

**Dockerfile.smaller**  
docker build -t go-smaller -f Dockerfile.smaller .  
docker image ls go-smaller  
docker run -ti --rm go-smaller  
