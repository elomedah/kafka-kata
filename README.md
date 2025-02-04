# kafka-kata


1- Ajouter les configurations kafka dans application.properties

````
spring.kafka.bootstrap-servers=ip_de_votre_server_kakfa:9092
spring.kafka.consumer.group-id=tp-kafka-step1
````


2- Creer un producteur

- Regrouper tout le code du producteur dans le package com.learn.kafka.producer
- Corriger la classe KafkaProducerConfig 
- Corriger également la classe MessageProducer 

3- Creer un consomateur

- Regrouper tout le code du consomateur dans le package com.learn.kafka.consumer
- Corriger la classe KafkaConsumerConfig
- Corriger également la classe MessageConsumer 

4- Pour vérifier que tout fonctionne bien, vous pouvez utilier le endpoint /produce pour envoyer des messages

```
curl --location --request POST 'http://localhost:8080/produce?content=message_content_here'

```

5- Changer de branche step-2.