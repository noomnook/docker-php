#Build
docker build -t [name] .
#Example
docker build -t docker-php .
#result is image file docker

#Run image file build after
docker run -d -p 80:80 -v [path source]:[path docker] [name]
#Example
docker run -d -p 80:80 -v ./src/:/var/www/html/ docker-php

-d, --detach                        Run container in background and
                                    print container ID
-p, --publish list                  Publish a container's port(s) to
                                    the host
-v, --volume list                   Bind mount a volume
More > docker run --help

https://hub.docker.com/_/php/