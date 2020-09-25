##

TODO:
Fix redis not working in docker


## How to build Boxclub App
1) Install docker
>> export DOCKER_HOST=127.0.0.1:2375
>> sudo reboot

2) commands
docker-compose up --build

  (run me in a different terminal v)
  docker-compose run backend rake db:migrate


## drop docker containers to reset state completely
docker-compose down
docker rm -f $(docker ps -a -q)
docker volume rm $(docker volume ls -q)






## Troubleshooting docker
https://github.com/docker/compose/issues/4181


https://nickjanetakis.com/blog/dockerize-a-rails-5-postgres-redis-sidekiq-action-cable-app-with-docker-compose
