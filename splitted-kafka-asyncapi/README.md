
#
## Create a json-schema file

## validate it with ajv

```
sudo npm install -g ajv-cli
sudo npm install -g ajv-formats
sudo npm install -g ajv-keywords
ajv validate -s schema/schema.json -d sample/sample1.json -c ajv-formats
```

## convert json-schema to avro






https://github.com/asyncapi/spec/blob/master/examples/streetlights-kafka.yml



https://microcks.io/blog/simulating-cloudevents-with-asyncapi/
https://github.com/microcks/microcks-quickstarters