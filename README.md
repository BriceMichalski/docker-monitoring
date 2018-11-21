TP-devops-docker-monitoring
===================

Practical school work for the implementation of a monitoring stack using
Elasticsearch, Fluentd and Kibana.

Prerequisites
------------
- install docker-ce
- install docker-compose

Used docker images
------------
- docker.elastic.co/elasticsearch/elasticsearch:6.4.3
- docker.elastic.co/kibana/kibana:6.4.3
- custom fluentD ( based on fluent/fluentd:v1.2.6 )( cf ./fulentd/Dockerfile)


Pull and build docker images
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
and Browse the kibana ihm http://localhost:5601

Stop
------------
```
$  docker-compose stop
```

fluentD listen port:
------------
- 5140 ( type: syslog , format: nginx )
- 24224 ( type: syslog , format: syslog, message_format: rfc5424 )


Useful links
------------
- ELK stack : https://www.elastic.co/elk-stack
- kibana : https://www.elastic.co/guide/en/kibana/6.4/index.html
- elasticsearch : https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html
- fluentd : https://docs.fluentd.org/v1.0/articles/quickstart
