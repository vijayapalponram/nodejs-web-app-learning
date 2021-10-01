# nodejs-web-app-learning

## Pre-requisites

- [nodejs](https://nodejs.org/en/download/)
- [docker](https://www.docker.com/products/docker-desktop)

## Running locally

### Install

Run the below command to install the dependencies.

```bash
npm install
```

### Serve

Run the below command to serve the application.

```bash
npm start
```

## Dockerization

You can run this nodejs application insider a docker.

### Building your image

Please run the below command for creating docker image from the root folder

```bash
docker build . -t vijayapal/nodejs-web-app-learning
```

### Run the image

Running your image with -d runs the container in detached mode, leaving the container running in the background. The -p flag redirects a public port to a private port inside the container. 

```bash
docker run -p 49160:8080 -d vijayapal/nodejs-web-app-learning
```

### Test

Test the application by using the url `http://localhost:49160`

## Reference

- [nodejs-docker-webapp](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)
