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
create table of "students" and "save"
![image](https://github.com/user-attachments/assets/b81c1ecd-83c5-4c10-8d71-13448cd0f42f)
now click on "public" in above line and you will get schema
![image](https://github.com/user-attachments/assets/5f23301c-2460-49e6-abfa-e8ac18f92250)
now go to "Alter TAble"
and enter some colums by clicking on "+" button
![image](https://github.com/user-attachments/assets/ab1ccd23-153d-415c-811f-4b1c7247aff7)





