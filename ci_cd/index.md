# Continuous Integration / Continuous Deployment

**Autor:** Leon Stümpeley

## CI/CD
* Bei jedem Push auf einen Main-Branch, wird dieser über einen Github Actions Workflow gebaut und in einem ausführbaren Docker Image gespeichert, dieser wird in einer Docker-Registry abgelegt.

* Nach ablegen eines Docker Images wird dieses im Running Enviroment deployed.

![](assets\ci_cd.png)
* Ausführen von Tests wird noch implementiert.

## Deployment-Komponenten
| Komponente          | Anbieter Wahl          |
|---------------------|------------------------|
| Deployment Umgebung | Ubuntu 20.04           |
| Reverse Proxy       | Traefik                |
| DNS Eintrag         | Name.com               |
| TLS Zertifikat      | Let's Encrypt          |
| Cloud Platform      | Digital Ocean Droplet  |
| Docker Registry     | Digital Ocean Registry |


* tls muss noch angebunden werden

## Reverse Proxy Konfiguration
* Die Zuordnung zum Micro-Service erfolgt über die Subdomain

| Micro-Service        	| Subdomain                      	                |
|----------------------	|-----------------------------------------------  |
| Landing Page         	| cyber-city.systems             	                |
| Verkehr              	| verkehr.cyber-city.systems     	                |
| Kultur               	| kultur.cyber-city.systems      	                |
| Gesundheitswesen     	| gesundheitswesen.cyber-city.systems           	|
| Umwelt               	| umwelt.cyber-city.systems      	                |
| Unternehmensregister 	| unternehmensregister.cyber-city.systems 	      |
| Authentifikation     	| auth.cyber-city.systems        	                |

* Auth ist momentan nicht implementiert

## Interne Host Adressen
| Micro-Service        	| Host                          	|
|----------------------	|--------------------------------	|
| Landing Page         	| cyber-city.systems             	|
| Verkehr              	| verkehr.cyber-city.systems     	|
| Kultur               	| kultur.cyber-city.systems      	|
| Gesundheitswesen     	| gesundheit.cyber-city.systems  	|
| Umwelt               	| umwelt.cyber-city.systems      	|
| Unternehmensregister 	| unternehmen.cyber-city.systems 	|
| Authentifikation     	| auth.cyber-city.systems        	|
