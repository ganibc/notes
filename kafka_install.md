Error running message:

[0.001s][warning][gc] -Xloggc is deprecated. Will use -Xlog:gc:/home/gani/work/kafka/bin/../logs/kafkaServer-gc.log instead.
Unrecognized VM option 'PrintGCDateStamps'
Error: Could not create the Java Virtual Machine.
Error: A fatal exception has occurred. Program will exit.

Solution:
Use java 8
sudo apt-get install openjdk-8-jdk
sudo apt-get install openjdk-8-jre
update-alternatives --config java


The install_kafka.md said clientPortAddress is 10.0.0.1
This only when the network interface IP address is 10.0.0.1
use 0.0.0.0 for local testing
clientPortAddress=0.0.0.0