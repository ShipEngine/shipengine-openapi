![OpenAPI Logo](https://shipengine.github.io/img/openapi-logo.png) ShipEngine™ OpenAPI Definition
==============================================

This repo contains [OpenAPI 3.0](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md) definitions for the [ShipEngine API](https://shipengine.com).  You can use these definitions with any of countless [OpenAPI tools](https://openapi.tools/) to generate sample code, tests, mock servers, etc.


Which file to use
-----------------------------------
Depending on your preferences and/or tooling, you may choose to use one or more of the following files:

|Path                |Description
|:-------------------|:--------------------------------
|[`src/openapi.yaml`](src/openapi.yaml)|This directory contains individual YAML files and folders for each API endpoint, request, response, and schema.  [`$ref` pointers](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#reference-object) are used to link from one file to another.<br><br> Many [OpenAPI tools](https://openapi.tools/) don't support multi-file API definitions, so you may need to use one of the single-file options below instead.
|[`openapi.yaml`](openapi.yaml)        |The entire ShipEngine OpenAPI definition, in a single YAML file.  This file uses [`$ref` pointers](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md#reference-object) to reduce duplication and keep the file small and fairly human-readable.<br><br> Some [OpenAPI tools](https://openapi.tools/) don't support YAML or don't support `$ref` pointers, so you may need to use the [`openapi.json` file](openapi.json) instead.
|[`openapi.json`](openapi.json)        |The entire ShipEngine OpenAPI definition, in a single JSON file.  This file **does not** contain any `$ref` pointers, which means it should work with any [OpenAPI tool](https://openapi.tools/).


Other API Definition Formats
-----------------------------------

### ![JSON Schema Logo](https://shipengine.github.io/img/json-schema-logo-small.png) JSON Schema
If you need to validate API requests and responses, then you may want to use [our JSON Schema definitions](https://github.com/shipengine/JSON-Schema).

### ![Postman Logo](https://shipengine.github.io/img/postman-logo-small.png) Postman
An official ShipEngine [Postman](https://getpostman.com) collection is **coming soon!**
