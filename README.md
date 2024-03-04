Start 3 broker cluster

1. Generate a uuid for cluster as follows:

./bin/kafka-storage.sh random-uuid

2. Use this uuid to run the following clusters as follows:

./bin/kafka-storage.sh format -t <cluster-uuid> -c config/Kraft/server-1.properties
./bin/kafka-storage.sh format -t <cluster-uuid> -c config/Kraft/server-2.properties
./bin/kafka-storage.sh format -t <cluster-uuid> -c config/Kraft/server-3.properties


Stop cluster gracefully:

./bin/kafka-server-stop.sh 