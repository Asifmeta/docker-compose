# docker-compose
How to use PostgreSQL with Docker & Python (also Web UI) Adminer
https://www.youtube.com/watch?v=nlk0QlPdbcY

# docker-compose
How to use PostgreSQL with Docker & Python (also Web UI) Adminer
https://www.youtube.com/watch?v=nlk0QlPdbcY

## 1st create compose file compose.yaml

        services:
        database:
            image: postgres
            restart: always
            ports:
            - "5432:5432"
            environment:
            - POSTGRES_USER=docker
            - POSTGRES_PASSWORD=docker
            - POSTGRES_DB=exampledb
        adminer:
            image: adminer
            restart: always
            ports:
            - "8080:8080"

