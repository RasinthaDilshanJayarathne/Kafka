# Kafka
<b>Kafka Commands</b>

.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

.\bin\windows\kafka-server-start.bat .\config\server.properties

.\bin\windows\kafka-topics.bat --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic cardApplicationRejectLetter
.\bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092
.\bin\windows\kafka-topics.bat --bootstrap-server localhost:9092 --topic TestTopic --describe

.\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic paymentFileValidate
.\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic eodParameterReset
.\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic cardReplace
.\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic eodAtmCashAdvanceUpdate
.\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic checkPaymentForMinimumAmount

.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic TestTopic --from-beginning

