Kong plugin bootstrap
====================

```
docker build . -t betchi/kong-plugin-bootstrap

docker run \
-v $PWD:/work \
-e "PLUGIN_NAME=kong-plugin-myplugin" \
-e "VERSION=0.1.0-1" \
betchi/kong-plugin-bootstrap
```