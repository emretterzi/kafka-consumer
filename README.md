# Kafka Consumer with Spring Boot

This is a simple Java Spring Boot application that serves as a Kafka Consumer. It demonstrates how to consume messages from a Kafka topic using the KafkaListener annotation and Spring Kafka integration.

## Prerequisites

- Java 8 or higher installed on your machine.
- Apache Kafka broker running on `localhost:9092`.

## Getting Started

1. Clone the repository to your local machine.
2. Ensure that Kafka is up and running on `localhost:9092`.
3. Build the application using Maven:
    ```bash
    mvn clean package
    ```
4. Run the application:
    ```bash
    java -jar target/kafka-consumer-app.jar
    ```

## Configuration

The application's configuration can be found in `application.properties`. You can update the following property as per your requirements:

- `kafka.topic`: The name of the Kafka topic from which messages will be consumed.

## Consumer Logic

The `ConsumerListener` class is the Kafka Consumer in this application. It listens to the Kafka topic specified in the configuration and consumes messages from it. The consumed messages are logged using the `@Slf4j` annotation.

## Notes

- The `@KafkaListener` annotation is used to specify the topic from which messages should be consumed.
- The `ConsumerRecord` object represents the consumed message and contains its key, value, and metadata.


## Author

- Emre Terzi
- GitHub:(https://github.com/emretterzi)
