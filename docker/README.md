# Warp4j

Turn JAR (java archive) into self-contained executable in a single command.

See project [page](https://github.com/guziks/warp4j) for more information.

## Usage

```
$ docker run --rm -it \
    -e "WARP4J_CACHE=/cache" \
    --volume <cache on host>:/cache \
    --volume <jars on host>:/workdir \
    --user $(id -u):$(id -g) \
    guziks/warp4j:stable <app.jar>
```

Change according to your requirements, but volume with working directory is mandatory.
