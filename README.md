# OpenAPI Specification sandbox

This repository is my sandbox of [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification).

Currently refer to Swagger.

## Mackerel API

- [mackerel-api.json](./mackerel/mackerel-api.json)

### Snipet

```sh
# C# Client
java -jar ./swagger-codegen-cli-2.3.1.jar generate \
   -i ./mackerel/mackerel-api.yml \
   -l csharp-dotnet2 \
   -o ./mackerel/client \
   --api-package Koudenpa.Mackerel.Api
```

```sh
# Node-RED Node
npm install
./node_modules/.bin/node-red-nodegen ./mackerel/mackerel-api.json \
    -o ./mackerel/node/ \
    --name mackerel-api-client \
    --keywords "nodered,mackerel" \
```
