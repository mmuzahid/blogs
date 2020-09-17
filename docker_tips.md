# Docker Tips

## Docker Commands

https://docs.docker.com/engine/reference/commandline/docker/

### docker info
- Display system-wide information
        
        docker info

### List of Images

        docker images
        
### List of containers
- List of Running Containers

        docker container ls

- List of All Containers
        
        docker container ls --all
       
### Start and Stop Container
- Start a container named `my-memcache`   
 
        docker start my-memcache
        
- Stop a container named `my-memcache`   
 
        docker stop my-memcache  

### Logs of a Container
- All Logs
        
        docker logs my-memcache

- Last few lines of Logs

        docker logs my-memcache --tail 10
        
        
