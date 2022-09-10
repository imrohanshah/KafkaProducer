Starting Kafka:

Creating Kafka docker:

- $ mkdir kafkaDocker
- $ kafkaDocker
- $ vim docker-compose.yml
    - Paste content from docker-compose file present in the project
- $ docker-compose up -d

Example request:

    curl --location --request POST 'localhost:8080/user/save' \
    --header 'Content-Type: application/json' \
    --data-raw '{
    "id":"imrohanshah",
    "name":"Rohan Shah",
    "age":23
    }'