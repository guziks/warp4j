# Warp4j

Turn Java application into self-contained executable. 

## Features

- automatically downloads JDKs
- creates custom runtimes optimized for your application
- creates self-contained binaries for Linux, MacOS and Windows using [warp-packer](https://github.com/dgiagio/warp)

## Install

TODO

## Usage

```bash
$ ls
my-app.jar

$ warp4j my-app.jar
...
...
...

$ ls
my-app.jar my-app-linux my-app-macos my-app.exe
```

## Cache Location

Downloaded JDKs and prepared bundles are here:

```bash
$HOME/.local/share/warp4j/
```
