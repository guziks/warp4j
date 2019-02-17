# Install

Here are several more ways to install `warp4j`.

## Manual

First install [warp-packer](https://github.com/dgiagio/warp/releases) and ensure other common tools available: `awk`, `curl`, `file`, `grep`, `sed`, `sort`, `tar`, `unzip`, optional: `zip`. Then install `warp4j` like this:

```
$ LOCATION=/usr/local/bin \
LINK=https://raw.githubusercontent.com/guziks/warp4j/stable/warp4j \
TEMP_LOCATION=/tmp/warp4j \
bash -c 'curl -fsSL -o $TEMP_LOCATION $LINK && \
sudo install -D \
  --mode=755 \
  --owner=root \
  --group=root \
  "$TEMP_LOCATION" "$LOCATION"'
```

Previous command can be also used to upgrade to the latest version.

## Docker

See docker hub [page](https://hub.docker.com/r/guziks/warp4j).

## Moor

Instead of direct `docker run` command you can make a launcher with [moor](https://github.com/guziks/moor):

```
$ moor guziks/warp4j:stable warp4j
```

Then use as an ordinary command.
