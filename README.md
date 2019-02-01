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

$ ls -1
my-app.jar
warped

$ ls warped
my-app-linux
my-app.linux-x64.tar.gz
my-app-osx
my-app.osx-x64.tar.gz
my-app-windows.exe
my-app.windows-x64.zip
```

See help:

```bash
$ wapr4j --help
```

## Cache Location

Downloaded JDKs and prepared bundles are here:

```bash
$HOME/.local/share/warp4j/
```
