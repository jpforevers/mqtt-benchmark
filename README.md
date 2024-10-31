
mqttx bench sub -v -h localhost -p 1883 -V 3.1.1 -c 10 -t abc/def/+ -q 1

mqttx bench pub -v -h localhost -p 1883 -V 3.1.1 -c 800 -im 100 -t abc/def/%c -q 1

./mqtt-benchmark --broker tcp://localhost:1883 --count 10000 --size 100 --clients 10 --qos 1

./mqtt-stresser-linux-amd64 -broker tcp://localhost:4883 -num-clients=10 -num-messages=10000
