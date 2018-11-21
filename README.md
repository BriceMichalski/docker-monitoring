# tp-docker-monitoring

Practical school work for the implementation of a monitoring stack using
Elasticsearch, Fluentd and Kibana.

Prerequisites :
------------
- install docker-ce
- install docker-compose
- install composer

Used docker images
------------
- docker.elastic.co/elasticsearch/elasticsearch:6.4.3
- docker.elastic.co/kibana/kibana:6.4.3
- custom fluentd ( based on fluent/fluentd:v1.2.6 )( cf ./fulentd/Dockerfile)


Pull and Build docker Image
------------
From project path run the following command:
```
$  docker-compose pull
$  docker-compose build
```

Start
------------
```
$  docker-compose up -d
```
and browse http://localhost:5601

Stop
------------
```
$  docker-compose stop
```
