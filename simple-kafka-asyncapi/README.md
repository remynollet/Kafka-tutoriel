### Create the asyncapi files
using vscode + asyncapi extension

Here, a good full exemple: asyncapi.yml

### Test spectral linter

```
npm install -g @stoplight/spectral-cli

create .spectral.yaml with line:
   extends: "spectral:asyncapi"

spectral lint asyncapi.yml
```

### Launch Kafka+microcks docker 

```
sudo service docker start
docker-compose up -d
docker ps -a
```

### Test microcks 

http:\\localhost:9090
use importer with the asyncapi.yml

### Have a look on kafdrop or AKHQ
Kafdrop:
http://localhost:9000

AKHQ:
http://localhost:9980


### Generate a Spring Cloud Stream project

```
npm install -g @asyncapi/generator
ag asyncapi.yml https://github.com/asyncapi/java-spring-cloud-stream-template -o cloud-stream
```
