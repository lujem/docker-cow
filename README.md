# Docker COW
COW (Climb Over the Wall) proxy on Docker

## Instruction
For run:
```sh
docker run \
--detach \
--restart=always \
--name=cow \
--volume=$HOME/.cow:/.cow \
--net=host \
nasermirzaei89/docker-cow \
/cow -rc=/.cow/rc
```
must mount rc path to container rc path.
