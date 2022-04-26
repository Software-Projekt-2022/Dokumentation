# Projektorganisation

**Autor:** Mark Mödeker

## Richtlinien

### Organisation

- Verwendetes Vorgehensmodell.
  - Vereinfachtes Scrum
- Welche Arten von Meetings finden wöchentlich statt?
  - Wöchentliches Meeting. Dienstags ab 14:30 bis Ende
  - Präsenz
- Geplanter Ablauf der Meetings.
  - Arbeitsfortschritt vorstellen
  - Workshops (Git und andere Techniken)
- Werkzeuge für Projektorganisation? Kanban-Board?
  - "Globales" Kanban-Board im Github
  - Optional: lokales Kanban-Board für jeden Microservice
- Wie läuft ein typischer Sprint ab?
  - Sprintlänge: 7 Tage
  - Retrospektivisch Sprintlänge veränderbar
- Wie sieht hier ein Codereview aus?
  - Software-Architekt macht Code-Review über Github-Issues und Kommentarfunktion
- Wie und womit wird die Teamkommunikation durchgeführt?
  - Discord
- Dokumentation:
  - Entwicklerdokumentation. On demand im Dokumentationsrepo.
  - Kundendokumentation. Nicht zwingend notwendig.
  - Meeting-Protokoll-Dokumentation. In diesem Dokumentationsrepo.
- Was ist der Produktlieferzeitplan? (x-Mal-wöchentliche Auslieferungen / Continuous I/D/D)
  - Jeder Commit führt zu einem Neu-Deployment
- Wie wird der Projektfortschritt gemessen und was passiert, wenn zeitlich verschoben werden muss?
  - Ziele im Github festlegen und Meilensteine ggfs. anpassen
- Wer setzt Erwartungen und Ziele fest und wie werden diese dokumentiert?
  - Zusammenspiel von Scrum-Master und Product-Owner
- Was passiert, wenn jemand Verbesserungsmöglichkeiten identifiziert?
  - Erstellt Issue an den Repo-Owner / Scrum-Master / Product-Owner
- Einschränkungen, Betriebsbedingungen, Faktoren und Risiken, die die Entwicklung beeinflussen können.
  - Krankheit
  - Andere Lehrveranstaltungen

### Team

- Werte und menschliche Umgangsformen
  - Respekt, Ausreden lassen, Höflichkeit
- Wie werden Meinungsverschiedenheiten gelöst?
  - Untereinander Konflikte lösen, danach an Scrum-Master eskalieren, danach an Dozent
- Wer legt Prioritäten und Zeitpläne fest?
  - Gesamtes Team
- Was passiert, wenn ein Teammitglied ein Ziel nicht einhält bzw. die Erwartungen nicht erfüllt?
  - Frühzeitige Bekanntgabe des Teammitglieds, der das Ziel nicht einhält
  - Direkte Ansprache an das Teammitglied, danach Eskalation

### Technik

- Interne Anforderungen an Softwarequalitätsmerkmale 
  - Erweiterbarkeit
  - Dokumentation
  - automatische und manuelle Tests
  - Statische Codeanalyse
  - Security
- Aufteilung in Repositories gemäß Systemarchitektur?
  - Je ein Repo für jeden Microservices
- Versionskontrolle? Git-Workflow?
  - Pro Sprint einen development-Branch
- Wie werden Änderungen integriert und ausgeliefert? CI/CD?
  - github-actions o.ä.
- Wie wird die Infrastruktur spezifiziert? Containerisierung?
  - docker
- für folgende Punkte ist jeder Software Engineer während der Implementierung selber verantwortlich:
  - Entwicklungsumgebung.
  - Betriebssysteme.
  - Programmiersprachen.
  - Frameworks.
  - Logging.
- Technologieauswahl: Messaging zum Beispiel mit [RabbitMQ](https://www.rabbitmq.com/) und [AsyncAPI](https://www.asyncapi.com/)

## Rollen und Verantwortlichkeiten

| Person | Rolle | Verantwortlichkeit |
|----------|-----------|-----------|
| Mark Mödeker | Scrum Master | Leitung, Kanban-Board, Protokollierung, Prozessqualität |
| Tim Bollmeyer | Product Owner | Produktvision, Integrations-Microservice ([Landing Page](landingpage/index)), Softwareproduktqualität |
| Leon Stümpeley | DevOps Engineer | Github-Repos, Docker, CI/CD, Dokumentation, Support, Infrastrukturqualität | 
| Andreas Wegner | Software Architekt | Technische Leitung/Vision, Code Reviews, Mentoring, Technikevaluation, Softwarequalität |
| Jonas vom Braucke | Software Engineer | Microservice [Verkehr](verkehr/index) |
| Toni Schnittger | Software Engineer | Microservice [Umwelt](umwelt/index) |
| Malte Kanders | Software Engineer | Microservice [Gesundheitswesen](gesundheitswesen/index) |
| Jason Piper | Software Engineer | Microservice [Authentifizierung](authentifizierung/index) |
| Clemens Maas | Software Engineer | Microservice [Unternehmensregister](unternehmensregister/index) |
| Mattis Fieseler | Software Engineer | Microservice [Kultur](kultur/index) |

## Grober Meilensteinplan

Zuästzlich zum Kanban-Board hier Meilensteine beschreiben.

**Feststehende Termine:**

* **Abgabe Spezifikation:** KW 16 (18.4.-20.4.)
* **Erster Prototyp (MVP):** KW 20 (16.5.-18.5.) / KW 21 (23.5.-25.5.)
* **Softwareprojektabgabe:** Ende Juni 2022 / Anfang Juli 2022
