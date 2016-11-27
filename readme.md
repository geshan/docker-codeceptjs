## Docker Container CodeceptJs with NightmareJs

This is a docker container for CodeceptJs with NightmareJs. It can be used to run
functional tests with NightmareJs or CodeceptJs. This image is based on node-slim.

[![](https://images.microbadger.com/badges/image/geshan/codeceptjs.svg)](https://microbadger.com/images/geshan/codeceptjs "Get your own image badge on microbadger.com")

## Pull it from docker registry

To pull the docker image you can do it with:

```
docker pull geshan/codeceptjs
```

## Usage

After pulling the image from docker registry, go into any project that has has the
codeceptjs tests, then run the following commands to run codeceptjs tests:

```
docker run -it -v $(pwd):/tests geshan/codeceptjs /bin/sh -c "xvfb-run codeceptjs run --steps"
```

## As base image

You can use it as a base image like below:

```
FROM geshan/codeceptjs

//my docker image contents
```
