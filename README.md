# kafka-spring-boot-getting-started
learned from this URL: very beginning
https://developer.confluent.io/get-started/spring-boot/#where-next

1. create topic:
docker exec broker \
kafka-topics --create \
--topic purchases \
--bootstrap-server localhost:9092 \
--replication-factor 1 \
--partitions 1

2. run producer:
   gradle bootRun --args='--producer'

2. run consumer:
   gradle bootRun --args='--consumer'
