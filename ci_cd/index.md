# Continuous Integration / Continuos Deployment

**Autor:** Leon Stümpeley

## CI
* Bei jedem Push auf einen Main-Branch, wird dieser über einen Github Actions Workflow gebaut und in einem ausführbaren Docker Image gespeichert, dieser wird in einer Docker-Registry abgelegt.

## CD
* Nach ablegen eines Docker Images wird dieses im Running Enviroment deployed.

## Deployment-Components
* Deployed in Docker Container

    ![](assets\docker.png)

* Github Repositories

    ![](assets\github.png)

* Deployment Server

    -> Ubuntu 20.04

    ![](assets\ubuntu.png)
    
    -> Digital Ocean Droplet

    ![](assets\digitalOcean.png)

* Database Server
    
    -> MySQL

    ![](assets/mysql.png)

* Reverse Proxy Server
    
    ->traefik proxy

    ![](assets/traefik.png)

* Docker Registry
    
    ->Private Digital Ocean Registry
    
    ->Eventueller Wechsel auf Public Docker Hub Registry

* DNS Entry
    
    ->cyber-city.systems (via name.com)

    ![](assets/name.com.png)

* TLS Certificate
    
    ->Automatic via letsencrypt

    ![](assets/letsencrypt.svg)

