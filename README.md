# xsoar-integration-internetdb

Simple Integration for the free [InternetDB-API](https://internetdb.shodan.io/)


## Note
Generate with openapi-codegen function from `demisto-sdk` & changed a little bit.

* [openapi.json](https://internetdb.shodan.io/openapi.json)

### Generate config for codegen

```bash
demisto-sdk openapi-codegen -i openapi.json -n InternetDB
ls -lah InternetDB_config.json
```

### Generate final python code

```bash
demisto-sdk openapi-codegen -cf InternetDB_config.json -i openapi.json -o output -n InternetDB
```

