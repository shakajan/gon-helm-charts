# gon-helm-charts

# Cassandra keyspace, table initialization
- 필요 동작: Cassandra가 ready 상태가 된 후 keyspace와 table을 생성
- 현재: 필요 동작이 가능한 상태에서 필요 동작을 수행하는 설정이 없음
- `https://github.com/Soongsil-Capstone-2024/cassandra.git`에 있는`scripts/init_cassandra.sh` 을 통해 keyspace와 table을 생성할 수 있음.

# Spark Application Submit
- 필요 동작: Spark가 ready 상태가 된 후 Application을 실행
- 현재: 필요 동작이 가능한 상태에서 필요 동작을 수행하는 설정이 없음
- `https://github.com/Soongsil-Capstone-2024/spark.git`의 `submit.sh`을 통해 Application을 실행시킬 수 있음.
- Application을 하기 전, kafka가 ready 상태이면서 topic을 가지고있어야함.

# Kafka topic
- 필요 동작: kafka가 ready 상태가 된 후 `/bin/kafka-topics`을 통해 `market` 토픽을 생성
- 현재: 필요 동작이 가능한 상태에서 필요 동작을 수행하는 설정이 없음
- kafka-0 shell에서 `/bin/kafka-topics --create --topic market --bootstrap-server kafka-0:9092 --partitions 1 --replication-factor 1`을 통해 생성할 수 있음.

