# sem03v24
Seminar 3 - 18.04.24


Ser på Docker Compose V2

docker compose
docker-compose

services:
    webtjeneste:
        image: nginx //siden vi ikke har nginx image på maskinen vil docker compose gjøre det for oss
        ports: 
         - "8080:80" //det er denne porten nginx skal kjøre på
        restart: always //sørger for at nginx alltid prøver å restarte hvis den går ned


//docker compose up //dette starter docker compose og kjører det
//localhost.8080 //dette er adressen som docker compose har laget for oss, skrives rett inn i nettleseren
