# tincancraft

## Build

	docker build -t minecraft .

## Run

First create a data volume

	docker volume create --name world

Then run the container to start the server

	docker run --name minecraft-base -d -p 25565:25565 -v world:/home/minecraft/world minecraft-base