# Kong plugin bootstrap

## Build docker image

```
docker build . -t betchi/kong-plugin-bootstrap
```

## Build lua package

```
docker run \
-v $PWD:/work \
-e "PLUGIN_NAME=kong-plugin-myplugin" \
-e "VERSION=0.1.0-1" \
betchi/kong-plugin-bootstrap
```

