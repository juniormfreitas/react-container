# wordpress-container

Docker environment made to run a Wordpress website project.

This repository will help you to run a Wordpress environment using Docker.

## Getting started

You must have Docker installed in your machine in order run this application in a Docker container.

If you don't have Docker installed please visit:

[Docker Official Website](https://www.docker.com/products/docker-desktop)

## The Environment

This is a simple wordpress environment containing Wordpress and MariaDB images.

Environment veriables are used in this project in order to make this infrastructure more flexible, the following varibales are used in the `.env` file.

```
APP_PORT
DB_PORT
DB_NAME
```

## Installing Wordpress

Make sure if your Docker is up and running in your computer.
Go to the root of this project where the `docker-compose.yml` file in placed then start the environment using the following command:

```
docker-compose up -d
```

The application will be placed in the `./src` folder automatically created if you don't have the `./src` folder and if you are running this command for first time. Wait until finish the download of all wordpress core files then you can go to the browser of your choice and access the following url:

```
http://localhost:8080
```

So you can create a wordpress website and start to develop new themes or new plugins.

To stop all the services you must run the following command:

```
docker-compose down
```
