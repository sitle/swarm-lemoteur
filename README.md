# Swarm - lemoteur

This repo allows to set up `lemoteur` in a Swarm cluster.


## Getting started

Deploy Elasticsearch stack

```
docker stack deploy -c docker-elasticsearch-stack.yml
```

Deploy Logstash stack

```
docker stack deploy -c docker-logstash-stack.yml
```

Deploy Kong stack

```
docker stack deploy -c docker-kong-stack.yml
```


