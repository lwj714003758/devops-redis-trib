## Docker Redis-trib

*jackeylov3/redis-trib* is a small Docker image based on [Alpine Linux](http://gliderlabs.viewdocs.io/docker-alpine/) providing Redis-trib.

*Redis-trib* is a command line tool executing commands to manage a Redis cluster


### Installation

1. Install [Docker](https://docs.docker.com/installation/#installation).

2. Download builded [image](https://registry.hub.docker.com/u/inem0o/redis-trib/) from public [Docker Hub Registry](https://registry.hub.docker.com/) 

		docker pull jackeylov3/redis-trib

### Build from source


	git clone https://github.com/lwj714003758/docker-redis-trib.git docker-redis-trib
	cd docker-redis-trib
	docker build -t redis-trib .
	docker run --rm redis-trib help

### Usage


	docker run --rm jackeylov3/redis-trib create --replicas 1 172.0.0.1:2000 172.0.0.2:2001 172.0.0.3:2002 


You can read more about Redis cluster and redis-trib tool here :

- [http://redis.io/topics/cluster-tutorial](http://redis.io/topics/cluster-tutorial)
- [http://redis.io/topics/cluster-spec](http://redis.io/topics/cluster-spec)
- [https://www.wanadev.fr/redis-3-0-le-cluster-de-nodes/ (french)](https://www.wanadev.fr/redis-3-0-le-cluster-de-nodes)
