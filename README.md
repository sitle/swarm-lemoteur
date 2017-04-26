# Swarm - lemoteur

This repo allows to set up `lemoteur` in a Swarm cluster.


## Getting started

Deploy Elasticsearch stack

```
docker stack deploy -c docker-elasticsearch-stack.yml elasticsearch
```

Deploy Logstash stack

```
docker stack deploy -c docker-logstash-stack.yml logstash
```

Deploy Kong stack

```
docker stack deploy -c docker-kong-stack.yml kong
```

Deploy lemoteur stack

```
docker stack deploy -c docker-lemoteur-stack.yml lemoteur
docker service update lemoteur_application --publish-add 3000:3000
```

## TODO

- [ ] Base template for elasticsearch and logstash: 1 ELK for logging and 1 ELK for application
- [ ] Placement constraints
- [ ] Docker secrets
