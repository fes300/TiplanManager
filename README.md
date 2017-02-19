# Progressive web app with authentication (Dockerized for development)

## Prerequisite technologies

- docker
- docker-compose

## Running it

Just clone the repository, run `npm install` and then `node server.js`.

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


## Running it with Docker compose

you need to have docker-compose installed. When you have it, just type `docker-compose up` from your terminal. it will do everything you need (use -d flag if you don't want to tail the logs of the containers).

If you want to rebuild the image use `docker-compose up --build`.


## AUTH-API

there's a README in the sub-folder

## FRONT-END

there's a README in the sub-folder
