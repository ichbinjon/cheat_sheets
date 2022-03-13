# Docker Cheat Sheet
`docker stop <containername>`

## See all containers
`docker ps`

`docker ps -a`

## Removing unneeded containers & images
`docker container prune && docker image prune`

OR in one command:

`docker system prune`

## Removing dangling `<none>` images
`docker rmi $(docker images -f "dangling=true" -q)`

## Running Postgres

https://hackernoon.com/dont-install-postgres-docker-pull-postgres-bee20e200198

`docker run --rm   --name pg-docker -e POSTGRES_PASSWORD=docker -d -p 5432:5432 -v $HOME/docker/volumes/postgres:/var/lib/postgresql/data  postgres`

https://nickjanetakis.com/blog/docker-tip-35-connect-to-a-database-running-on-your-docker-host

`ipconfig getifaddr en0` for local IP address over wifi

`ipconfig getifaddr en0` for local IP over ethernet


https://stackoverflow.com/questions/54657006/smtpauthenticationerror-5-7-14-please-log-n5-7-14-in-via-your-web-browser