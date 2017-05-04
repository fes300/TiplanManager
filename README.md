# Progressive web app with authentication (Dockerized for development)

## Prerequisite technologies

- docker
- docker-compose

## Getting the code

Just clone the repository with `git clone git@bitbucket.org:fes300/tiplan-manager.git`
init the submodules with `git submodule init`
and lastly update the submodules with `git submodule update`.


## Running it with Docker compose

you need to have docker-compose installed. When you have it, just type `docker-compose up` from your terminal. it will do everything you need (use -d flag if you don't want to tail the logs of the containers).

If you want to rebuild the image use `docker-compose up --build`.

N.B.: if something goes wrong somewhere there's a chance that Docker cache will remain "dirty" and it could try to use images that don't exist anymore. If this happen just clean it up with `docker-compose down`.


## Useful Docker commands

to check the logs of a running container (tail):
`docker logs -f [container-id]`

to run a bash shell inside a running container:
`docker exec -it [container-id] bash`

after you created the container you just start/stop it with
`docker stop [container-id]`
`docker start [container-id]`

to remove a container:
`docker rm [container-id]` (use -f to force)

to remove an image:
`docker rmi [image-id]` (use -f to force)

remove all images and containers created by a `docker-compose up` command
`docker-compose down -v --rmi all`



## AUTH-API

there's a README in the sub-folder

## FRONT-END

there's a README in the sub-folder