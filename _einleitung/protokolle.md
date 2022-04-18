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
