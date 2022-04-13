# Continuous Integration / Continuos Deployment

**Autor:** Leon Stümpeley

## CI
* Bei jedem Push auf einen Main-Branch, wird dieser über einen Github Actions Workflow gebaut und in einem ausführbaren Docker Image gespeichert, dieser wird in einer Docker-Registry abgelegt.

## CD
* Nach ablegen eines Docker Images wird dieses im Running Enviroment deployed.

## Deployment-Components
* Github Repositories

* Deployment Server

    -> Digital Ocean Droplet

* Database Server
    
    ->Digital Ocean Database

* Proxy Server
    
    ->traefik proxy

* Docker Registry
    
    ->Private Digital Ocean Registry
    
    ->Eventueller Wechsel auf Public Docker Hub Registry

* DNS Entry
    
    ->cyber-city.systems (via name.com)

* TLS Certificate
    
    ->Automatic via letsencrypt

