# OpenAPI Specification sandbox

This repository is my sandbox of [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification).

Currently refer to Swagger.

## Mackerel API

- https://github.com/7474/mackerel-openapi-spec

### Snipet

```sh
# C# Client
npm install
npm run openapi-generator -- generate \
   -i ./mackerel/mackerel-api.yml \
   -g csharp-dotnet2 \
   -o ./mackerel/client \
   --api-package Koudenpa.Mackerel.Api
```

```sh
# Node-RED Node
npm install
npm run node-red-nodegen -- ./mackerel/mackerel-api.json \
    -o ./mackerel/node/ \
    --name mackerel-api-client \
    --keywords "nodered,mackerel"
```
