# Wetter

**Autor:** Toni Schnittger


## Überblick

Im Microservice Wetter sollen die Temperatur, die Luftreinheit, das Wetter, der Pollenflug, klarheit des Himmels sowie der Wasserstand des Stadt nahen Flusses 
übersichtlich für verschiedene Stadtteile dargestellt werden. Außerdem sollen passend zu den verhältnissen Aktivitäten wie z.B. Radfahren vorgeschlagen werden.
Wichtig sollte dazu noch eine Warnung zu bevorstehendem Extremwetter wie Stürme oder Hochwasseer sein. Der Microservice soll die Nutzer mit allem verbinden was
Wettertechnisch in der Stadt passiert. 

- Textuelle Beschreibung der Anwendungsdomäne
- Konzeptionelles Analyseklassendiagramm (logische Darstellung der Konzepte der Anwendungsdomäne)


## Funktionale Anforderungen

* Definition der Akteure
* Use-Case Diagramme
* Strukturierung der Diagramme in funktionale Gruppen
* Akteure sowie andere Begriffe der implementierten Fachdomäne definieren 
* Begriffe konsistent in der Spezifikation verwenden  
* Begriffe im Glossar darstellen

Akteure: Alle Bürger oder Touristen mit Interesse am Wetter


## Anforderungen im Detail

- User Stories mit Akzeptanzkritierien 
- Optional: Name (oder ID) und Priorität ("Must", "Should", "Could", "Won't")
- Strukturierung der User Stories in funktionale Gruppen
- Sicherheit: Misuse-Stories formulieren


**Beispiel 1**

| **Als** | **möchte ich** | **so dass** | **Erfüllt wenn** | **Priorität**   |
| :------ | :----- | :------ | :-------- | :-------- |
| Sportler | wissen ob es heute regnet | ich nicht vom Regen überrascht werde | Wetter für den rest des Tages angezeigt wird | Muss |
| Allergiker | wissen welche Pollen-Arten fliegen | ich weiß ob ich Medikamente nehmen muss | Anzeige für Pollenflug/Arten | Muss |
| Angler | den Wasserstand erfahren | ich weiß ob ich Angeln gehen kann | Wasserstand anzeige | Muss |


## Graphische Benutzerschnittstelle

- GUI-Mockups passend zu User Stories
- Screens mit Überschrift kennzeichnen, die im Inhaltsverzeichnis zu sehen ist
- Unter den Screens darstellen (bzw. verlinken), welche User Stories mit dem Screen abgehandelt werden
- Modellierung der Navigation zwischen den Screens der GUI-Mockups als Zustandsdiagramm
- Mockups für unterschiedliche Akteure

**Wetter Startseite**

![Mockup01](https://github.com/Software-Projekt-2022/Dokumentation/edit/Unterseite-Infrastruktur_Wetter/wetter/media/Wetter_Mockup01.png)

## Datenmodell 

Eine Datenbank wird für den Wetter Microservice nicht benötigt, da die Vergangenen Wetterdaten ebenfalls über die API verfügbar sind.

## Abläufe

- Aktivitätsdiagramm für den Ablauf sämtlicher Use Cases
- Aktivitätsdiagramme für relevante Use Cases
- Aktivitätsdiagramm mit Swimlanes sind in der Regel hilfreich 
  für die Darstellung der Interaktion von Akteuren der Use Cases / User Stories
- Abläufe der Kommunikation von Rechnerknoten (z.B. Client/Server)
  in einem Sequenz- oder Aktivitätsdiagramm darstellen
- Modellieren Sie des weiteren die Diagramme, die für das (eigene) Verständnis des
  Softwaresystems hilfreich sind. 
  
  
  Wetter abfrage alle 15 Minuten, Pollen Täglich jeden Morgen, Wasserstand alle 30 Minuten


## Schnittstellen

- Schnittstellenbeschreibung (API), z.B. mit OpenAPI 
- Auflistung der nach außen sichtbaren Schnittstelle des Microservices. Über welche Schnittstelle kann z.B. der Client den Server erreichen?
- In Event-gesteuerten Systemen ebenfalls die Definition der Ereignisse und deren Attribute
- Aufteilen in Commands, Events, Queries
* Abhängigkeiten: Liste mit Kommunikationsabhängigkeiten zu anderen Microservices

API: 
Wetter, UV-Level, etc: Openweathermap(https://openweathermap.org/api) 
Wasserstand: Pegelonline(https://www.pegelonline.wsv.de/webservice/dokuRestapi)
Pollen: Pollen Forecast API(https://achoo.dev/)

**Beispiel:**

### URL

http://smart.city/microservices/wetter

### Commands

**Synchronous**



**Asynchronous**

| **Name** | **Parameter** | **Resultat** |
| :------ | :----- | :------ |
| createContract() | int id | int id |
| changeContract() | int id | - |

### Events

**Customer event channel**

| **Name** | **Payload** | 
| :------ | :----- | 
| Customer Authorized | int id |
| Customer Deleted | int id |

**Contract event channel**

| **Name** | **Payload** | 
| :------ | :----- | 
| Contract Received | int id |
| Contract Deleted | int id |

### Queries

| **Name** | **Parameter** | **Resultat** |
| :------ | :----- | :------ |
| getWeather() | - | JSON weatherdata |
| getPollen() | - | JSON Pollendata |

### Dependencies

#### RPC

| **Service** | **Funktion** |
| :------ | :----- | 
| Authorization Service | authenticateUser() |
| Hospital Service | blockDate() |

#### Event-Subscriptions

| **Service** | **Funktion** |
| :------ | :----- | 
| Cinema channel | CancelFilmCreatedEvent |
| Customer reply channel | CreateCustomerEvent |


## Technische Umsetzung


### Softwarearchitektur

- Darstellung von Softwarebausteinen (Module, Schichten, Komponenten)

Hier stellen Sie die Verteilung der Softwarebausteine auf die Rechnerknoten dar. Das ist die Softwarearchitektur. Zum Beispiel Javascript-Software auf dem Client und Java-Software auf dem Server. In der Regel wird die Software dabei sowohl auf dem Client als auch auf dem Server in Schichten dargestellt.

* Server
  * Web-Schicht
  * Logik-Schicht
    - Javascript 
  * Persistenz-Schicht

* Client
  * View-Schicht
    - HMTL
    - CSS
  * Logik-Schicht
    - Javascript
  * Kommunikation-Schicht

Die Abhängigkeit ist bei diesen Schichten immer unidirektional von "oben" nach "unten". Die Softwarearchitektur aus Kapitel "Softwarearchitektur" ist demnach detaillierter als die Systemübersicht aus dem Kapitel "Systemübersicht". Die Schichten können entweder als Ganzes als ein Softwarebaustein angesehen werden. In der Regel werden die Schichten aber noch weiter detailliert und in Softwarebausteine aufgeteilt. 



### Entwurf

- Detaillierte UML-Diagramme für relevante Softwarebausteine

### Fehlerbehandlung 

* Mögliche Fehler / Exceptions auflisten
* Fehlercodes / IDs sind hilfreich
* Nicht nur Fehler technischer Art ("Datenbankserver nicht erreichbar") definieren, sondern auch fachliche Fehler wie "Kunde nicht gefunden", "Nachricht wurde bereits gelöscht" o.ä. sind relevant. 

* Server einer API sind nicht erreichbar

### Validierung

* Relevante (Integrations)-Testfälle, die aus den Use Cases abgeleitet werden können
* Testfälle für 
  - Datenmodell
  - API
  - User Interface
* Fokussieren Sie mehr auf Integrationstestfälle als auf Unittests
* Es bietet sich an, die IDs der Use Cases / User Stories mit den Testfällen zu verbinden,
  so dass erkennbar ist, ob Sie alle Use Cases getestet haben.

### Verwendete Technologien

- Verwendete Technologien (Programmiersprachen, Frameworks, etc.)

* Frontend
  - HTML
  - CSS
  - 
* Backend
  - REST API
  - Javascript
* Datenbank
