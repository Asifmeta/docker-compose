# docker-compose
Folder path on my system
C:\Users\Asif sb\Desktop\code\docker\docker-compose

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

Then run below commands 
* docker compose config
* docker compose up
  * two images with name "postgres" and "adminer" created
  * Also main container named "docker-compose" and sub container with name "postgres" and "adminer" created

 Now open port http://127.0.0.1:8080/
 serername =  servicename 
 and all other details as per below picture
![image](https://github.com/user-attachments/assets/89547821-9553-4e2f-b46d-1841da24a879)
click on login button
![image](https://github.com/user-attachments/assets/3554eaa7-09c9-4d94-b538-8f96b78f0fd0)


