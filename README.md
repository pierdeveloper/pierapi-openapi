# PierAPI OpenAPI

## Overview
This repository contains the OpenAPI spec so that anyone can generate a client to call Pier's APIs. Some common tools are [OpenAPI Generator](https://openapi-generator.tech/) and [Swagger Codegen](https://swagger.io/tools/swagger-codegen).

## Generate Client
The following is an example on how to generate the `typescript-axios` SDK using `openapi-generator` on Mac:
```bash
brew install openapi-generator
openapi-generator generate \
  -i sdk-api.yaml \
  -g typescript-axios \
  -o ./stage-typescript \
  --additional-properties=npmName=stage-typescript,supportsES6=true
```

## More Information
For more information please see Pier's docs [docs](https://docs.pier-finance.com/).
