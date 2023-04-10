## __Title: pistache-json-api-base__
#### Author:
- Chimera Kang

**NOTE**: This script requires Docker installation ( more info on https://docs.docker.com/engine/install/ ).

## How to Install
- Test your Docker installation
```
$ docker --version
$ docker run hello-world
```
- If Docker is correctly installed, execute the following commands:
```
$ cd docker
$ ./build.sh
```
## How to use:
- Execute the following command to start the server :
```
$ docker-compose up
```
## How to test (using curl):
- Chart - Endpoint /market-data/chart
```
$ curl -X GET http://127.0.0.1:9080/market-data/chart -d '{"providers": ["CBOE"]}'
$ curl -X GET http://127.0.0.1:9080/market-data/chart -d '{"providers": ["CBOE", "UBS"], "pair": "EUR/GBP", "start" : "2019-10-05 18:00:00", "end": "2020-06-08 21:17:00"}'
```
