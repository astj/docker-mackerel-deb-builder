# mackerel-deb-builder

## What's this

This Docker image is used to build deb packages in Dockernized envirionment.

This image is intended to build [mackerel-agent](https://github.com/mackerelio/mackerel-agent), but maybe you can use this image to build another packages.

## Usage

Use `docker run ...` instead of `debuild` command.

Following example will work as `debuild -uc` on `$(PWD)/deb-build`.

```
$ docker run --rm "$(PWD)":/workspace -w /workspace/deb-build astj/mackerel-rpm-builder:d8 -uc
```

## Tags

TBD (We'd like to provide `d8`, `d9`, ...)
