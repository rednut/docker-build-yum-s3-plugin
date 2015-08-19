# Build yum-s3-plugin rpm package using docker

This docker container will build an rpm package for `yum-s3-plugin` and drop the resulting rpm into the `/data` path / volume.


# Usage


## Make a folder for the rpm output

```
  mkdir -p $PWD/yum-s3-plugin-builder 
```

## Build me an rpm package for yum-s3-plugin

```
  docker run \
    -i -t --rm \
    -v $PWD/yum-s3-plugin:/data \
      rednut/yum-s3-plugin-builder
```

## Check output

:-)


