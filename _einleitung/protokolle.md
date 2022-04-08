## 08.04.2022 17:30 - 18:00
### Teilnehmer:
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

### Themen:
* Microservice Zuteilung

| Teilnehmer | Microservice |
| - | - |
| Jonas | Verkehr |
| Malte | Gesundheitswesen |
| Mattis | Kultur |
| Toni | Wetter |
| Jason | Infrastruktur |
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
