# Docker COW

COW (Climb Over the Wall) proxy on Docker

[![](https://img.shields.io/docker/cloud/build/nasermirzaei89/cow.svg)](https://hub.docker.com/r/nasermirzaei89/cow/builds)
[![](https://images.microbadger.com/badges/image/nasermirzaei89/cow.svg)](https://microbadger.com/images/nasermirzaei89/cow)
[![](https://img.shields.io/docker/pulls/nasermirzaei89/cow.svg)](https://hub.docker.com/r/nasermirzaei89/cow)

## Instruction

### Run:

```bash
docker run \
--detach \
--restart=always \
--name=cow \
--volume=$HOME/.cow:/.cow \
--net=host \
nasermirzaei89/cow \
/cow -rc=/.cow/rc
```

You must mount `rc` path to container `rc` path.
