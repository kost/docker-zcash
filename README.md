# k0st/zcash

Zcash inside docker

Image is based on the [debian](https://hub.docker.com/_/debian/) base image

## Docker image size

[![Latest](https://badge.imagelayers.io/k0st/zcash.svg)](https://imagelayers.io/?images=k0st/zcash:latest 'latest')

## Docker image usage

```
docker run [docker-options] k0st/zcash
```

## Examples

Typical basic usage (start zcashd daemon): 

```
docker run -it k0st/zcash zcashd
```

Typical usage to mine:

```
docker run -it k0st/zcash zcashd -gen
```

Typical usage to perform query:

```
docker run -d --name zcash test/zcash zcashd
docker exec -u zcash zcash zcash-cli getbalance
```

### Todo
- [ ] Perform more testing

