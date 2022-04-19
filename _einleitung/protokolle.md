# Protokolle
Autor: Mark Mödeker

## 08.04.2022 17:30 - 18:00
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Jonas vom Braucke | Software Engineer |
| Clemens Maas | Software Engineer |
| Jason Piper | Software Engineer |
| Mattis Fieseler | Software Engineer |
| Malte Kanders | Software Engineer |
| Toni Schnittger | Software Engineer |

### Themen
* Microservice Zuteilung

| Teilnehmer | Microservice |
| - | - |
| Jonas | Verkehr |
| Malte | Gesundheitswesen |
| Mattis | Kultur |
| Toni | Wetter, Infrastruktur |
| Jason | Authentifizierung |
| Clemens | Unternehmensregister |

* erster Sprint
  * 11 Tage statt 7
  * die Softwarespezifikation fertigstellen
  * Kanban Board wird aktuell noch vorbereitet
  * Kleines Daily Scrum am Dienstag 12.04.2022 zum zwischenstand präsentieren
* Wie sollen die Microservices kommunizieren
* RabbitMQ
* Welches Protokoll wollen wir zum versenden der Daten verwenden? Aktuell: JSON
* Welche Events wären nützlich für die Microservices? 
  * Events können mit ASYNC API Dokumentiert werden
  * Am Dienstag besprechen wir weiter inwiefern die Services miteinander interagieren
  * jeder Software Engineer soll sich bis dahin Gedanken machen welche Events für ihn nützlich wären
* Jeder Microservice soll direkt mit dem Gedanken designed werden, dass wir Single-Sign-On einsetzen wollen
  * Wie wollen wir eine gemeinsame Schnittstelle realisieren für Single-Sign-On
* Jeder Mitwirkende muss ungefähr gleichen Aufwand am Ende des Projektes haben

## 12.04.2022 14:30 - 16:00
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Jonas vom Braucke | Software Engineer |
| Clemens Maas | Software Engineer |
| Jason Piper | Software Engineer |
| Mattis Fieseler | Software Engineer |
| Malte Kanders | Software Engineer |
| Toni Schnittger | Software Engineer |

### Themen
* Pünktlichkeit ist die Höflichkeit der Könige
* Vorstellung Kanban Board und erster Sprint
  * Präsentieren der Ideen die sich Scrum Master und Product Owner über die Woche gemacht haben
  * im Github Projects
  * Issues haben alle kleine Akzeptanzkriterien
  * Fragen
* Spezifikationskriterien
* Wird die Authentifizierung ein eigener Service?
  * Wird es überhaupt benötigt? Pro und Contra Diskussion
  * Legen wir andere Themen zusammen damit ein Engineer die Auth übernehmen kann?
  * Authentifizierung komplexer als nur username und password:
    * 2 Faktor Authentifizierung
    * E-Mail Bestätigung
  * Wetter und Infrastruktur werden zusammengelegt, Authentifizierung durch Jason
* Datenspeicherung
  * Benötigen wir diese als extra Service? Pro und Contra Diskussion
* Zwischentermin Findung: 15.04.2022 14 Uhr, 16.04.2022 14 Uhr
* AsyncAPI: Fragen zur Umsetzung
* RabbitMQ: Fragen zur Umsetzung
  * Eventuell anderen Service nutzen Pro Contra
  * Wie funktioniert RabbitMQ
  * Validierung, Tests inwiefern setzen wir das um
  * mindestens Exceptionhandling bei fehlerhaften Events
* CI/CD
  * Wie setzen wir die Docker Container um
  * Der DevOps Engineer übernimmt alle Container und Deployed jeden Main Branch
  * Wie wird man auf die einzelnen Services weitergeleitet?
    * Jeder Service eigene Domain, Verlinkung auf der Landing Page
    * Subdomains
    * eine Domain und die Microservices dann auf Unterseiten
* Welche Sprachen wollen die einzelnen Software Engineers verwenden?
  * Python, MySQL(ite)
  * Java, Springboot
  * Java, MySQL
  * Kotlin, Springboot
  * Java
  * JavaScript, MariaDB
* Namensänderung von Smart City in CyberCity - angenommen
* Fragen und Bedenken zum 1. Sprint

## 15.04.2022 14:00 - 16:00
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Clemens Maas | Software Engineer |
| Malte Kanders | Software Engineer |
| Toni Schnittger | Software Engineer |
| später erschienen |
| Andreas Wegner | Software Architekt |
| Jonas vom Braucke | Software Engineer |

### Themen
* Was wird heute alles besprochen
  * Wir schauen uns den bisherigen Stand der Mitglieder an
  * Geben Feedback zu den bisherigen Spezifikationen
* Clemens stellt seine Spezifikation vor
* Toni stellt seine Spezfikation vor
* Malte stellt seine Spezifikation vor
* Kleinere Fahrplanbesprechung
* Jonas und Mattis mit Karte absprechen
* Punkte in Spezifikationen -> Validierung? Softwarearchitektur vs. Verwendete Technologien (eins von beiden raus schmeißen?!)
* Andreas stellt ein RabbitMQ Beispiel vor
* PO und SM bereiten ein globales Stylesheet vor
* Jonas stellt eine Seite vor die Farben und Fonts vorschlägt
* "Wetter/Infrastruktur" heißt jetzt "Umwelt"

## 16.04.2022 14:00 - 15:50
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Jonas vom Braucke | Software Engineer |
| Jason Piper | Software Engineer |

### Themen
* Was wird heute alles besprochen
  * Wir schauen uns den bisherigen Stand der Mitglieder an
  * Geben Feedback zu den bisherigen Spezifikationen
* Jason stellt seine Spezifikation vor
* Jonas stellt seine Spezifikation vor
* kleine Fragen/Antworten Runde
* Leon stellt seine Spezifikation vor
  * Erklärung zu Traefik
  * Besprechung zum Deployment bei DigitalOcean
* Diskussion zu RabbitMQ
* Muss man sich noch gegenseitig helfen bei den Spezifikationen
* Wo bekommt Andreas die Variablen für die Events her
* Roadmap Besprechung

## 19.04.2022 14:30 - 
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Jonas vom Braucke | Software Engineer |
| Clemens Maas | Software Engineer |
| Jason Piper | Software Engineer |
| Mattis Fieseler | Software Engineer |
| Malte Kanders | Software Engineer |
| Toni Schnittger | Software Engineer |

## Themen
* Vorstellung der Spezifikationen
  * Projektübersicht
    * In Diagrammen immer mit Pfeilen arbeiten
  * Projektorganisation
    * Nicht viel hinzugekommen, nur die korrekten Microservice einteilungen und deren Verlinkungen
  * Protokolle
  * CI/CD
    * Titel der Seite korrigieren
    * Testing aufnehmen in die Arbeitsschritte
    * Neben MySQL jetzt noch PostgreSQL
    * Datenbanken in Containern
    * Entwickler müssen ihre Technologien und Ports für den DevOps Engineer dokumentieren
    * Sollten die Software Engineers ihre Docker Files selber schreiben?
  * Events
    * an einem JSON example wird erklärt wie der Eventbus aussehen wird
    * Wie vollständig ist die Spezifikation? Wird noch ausgebaut, es werden noch mehr Events von den Software Engineers benötigt.
  * Landing Page
  * Authentifizierung
  * Verkehr
    * Inwiefern funktioniert die Autorisirung pro Microservice?
  * Umwelt
    * Denglisch generell nicht erwünscht (Hier bei Umwelt kein Fehler).
  * Gesundheitswesen
    * Weitere spalte in den Anforderungen hinzufügen für muss/soll/kann
  * Unternehmensregister
    * Tabelle richtig formatieren
  * Kultur
    * Leaflet js um die Karte anzuzeigen
* Nachbesprechung 1. Sprint
  * Was lief gut
    * Kommunikation
    * Jede Person hat seine Aufgaben weitesgehend geschafft
  * Was lief schlecht
    * Kanban Board
    * gesplittete Meetings vermeiden damit alle immer den gleichen Informationsstand haben
* Kanbanboard Kritik und Feature Vorstellung
  * Die eigenen Issues immer aktuell halten
  * Eventuell den eigenen Namen filtern damit es nicht so viele Aufgaben sind
  * Manche Aufgaben zu grob, andere sehr spezifisch -> Gute Balance finden
  * Häkchen teilweise ein Arbeitsschritt zu viel, sollte eher zur Orientierung dienen und nicht Pflicht sein
  * Weitere Tasks während der Implementierung aufgegriffen
* Rollen und Verantwortlichkeiten
  * Product Owner
    * Nur WAS gemacht wird, nicht WIE etwas gemacht wird?
    * Der PO sollte weiterhin auch Vorschläge zum WIE einbringen können
    * Muss eine klare Produktvision im Kopf haben
    * Kann eingreifen wenn etwas nicht mit der Vision übereinstimmt
  * Abgrenzung DevOps Engineer und Software Architekt
    * Der Software Architekt hat die Idee, der DevOps Engineer übernimmt die Umsetzung
    * Reverse Proxy wird vom DevOps Engineer umgesetzt
  * Scrum Master
    * Starker Fokus auf Prozessqualität in den nächsten Schritten
    * Einen gemeinsamen Workflow umsetzen
* Mehr als ein Meeting?
  * In der Anfangsphase eher nicht, aber zum Abschluss des Projektes mehr Besprechungen
  * Mehrere Termine können zu Komplikationen führen mit den normalen Terminen der Gruppenmitglieder
  * Kürzere Termine sollten schneller zu finden sein als Stundenlange
* Pull Requests umsetzung
  * Software Architekt muss die Code Reviews durchführen, muss bitte Assigned werden
  * DevOps Engineer muss die main branches protecten, nur über Pull Request können Änderungen darauf kommen
  * Was wird alles reviewed? 
* Andreas braucht ein eigenes Repository für Beispiele, etc.
* Event Spezifikation automatisiertes Deployment funktioniert nicht
* Sprintplanning extra Informationen und Diskussionsstoff
  * wieder 7 Tage
  * wie soll der Entwicklungsbranch heißen? Dev-Branch/Sprint-Branch/Feature-Branch: Ein Dev-Branch wochenübergreifend
  * Ein Dev-Branch von dem Features-Branches abgezweigt werden können. Nur der Dev-Branch wird am Ende des Sprints in den Main-Branch gemerged.
  * Eventueller Docker Workshop? Abgelehnt.
  * Beispieldaten nur für Testfälle oder auch für die Implementierung
  * Beispieldaten sollten zusammenhängend funktionieren
* Arbeitsaufwand für eine Woche gerechtfertigt?
  * Im Allgemeinen ein schaffbarer Sprint
