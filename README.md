# xsoar-integration-internetdb

Simple Integration for the free [InternetDB-API](https://internetdb.shodan.io/)

![image](https://github.com/dbiesecke/xsoar-integration-internetdb/assets/8032783/b9d4a759-b9fb-457c-a199-93de03f59ccf)

## Install

Upload [InternetDB.yml](https://raw.githubusercontent.com/dbiesecke/xsoar-integration-internetdb/main/InternetDB.yml) to your Instance & activate it

![image](https://github.com/dbiesecke/xsoar-integration-internetdb/assets/8032783/42174bac-8993-4b02-a543-d5020d57e54d)

* No API KEY NEEDED!


## internetdb-info-ip-get 

  * ip={{IP}}  (Mandatory)



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

