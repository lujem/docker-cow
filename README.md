# Docker COW

COW (Climb Over the Wall) proxy on Docker

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
