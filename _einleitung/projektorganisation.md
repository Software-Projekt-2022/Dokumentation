# Projektorganisation

**Autor:** Scrum Master: Mark Mödeker

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
- Wie und womit wird die Teamkommunikation durchgeführt?
- Dokumentation:
  - Entwicklerdokumentation?
  - Kundendokumentation?
  - Meeting-Protokoll-Dokumentation?
- Was ist der Produktlieferzeitplan? (x-Mal-wöchentliche Auslieferungen / Continuous I/D/D)
- Wie wird der Projektfortschritt gemessen und was passiert, wenn zeitlich verschoben werden muss?
- Wer setzt Erwartungen und Ziele fest und wie werden diese dokumentiert?
- Was passiert, wenn jemand Verbesserungsmöglichkeiten identifiziert?
- Einschränkungen, Betriebsbedingungen, Faktoren und Risiken, die die Entwicklung beeinflussen können.

### Team

- Werte und menschliche Umgangsformen
- Wie werden Meinungsverschiedenheiten gelöst?
- Wer legt Prioritäten und Zeitpläne fest?
- Was passiert, wenn ein Teammitglied ein Ziel nicht einhält bzw. die Erwartungen nicht erfüllt?

### Technik

- Interne Anforderungen an Softwarequalitätsmerkmale 
  - Erweiterbarkeit
  - Dokumentation
  - automatische und manuelle Tests
  - Statische Codeanalyse
  - ...
- Aufteilung in Repositories gemäß Systemarchitektur? Monorepo?
- Versionskontrolle? Git-Workflow?
- Wie werden Änderungen intgriert und ausgeliefert? CI/CD? 
- Wie wird die Infrastruktur spezifiziert? Containerisierung?
- Implementierung
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
| Tim Bollmeyer | Product Owner | Produktvision, Integrations-Microservice, Softwareproduktqualität |
| Leon Stümpeley | DevOps Engineer | Github-Repos, Docker, CI/CD, Dokumentation, Support, Infrastrukturqualität | 
| Andreas Wegner | Software Architekt | Technische Leitung/Vision, Code Reviews, Mentoring, Technikevaluation, Softwarequalität |
| Jonas vom Brauke | Software Engineer | Microservice [Parkplatz](parkplatz/index) |
| Toni Schnittger | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |
| Malte Kanders | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |
| Jason Piper | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |
| Clemens Maas | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |
| Mattis Fieseler | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |
| Eric Neppert | Software Engineer | Microservice [Krankenhaus](krankenhaus/index) |

Hinweis: Ein Microservice für die Authentifizierung/Autorisierung könnte sinnvoll sein.

## Grober Meilensteinplan

Zuästzlich zum Kanban-Board hier Meilensteine beschreiben.

**Feststehende Termine:**

* **Abgabe Spezifikation:** KW 16 (18.4.-20.4.)
* **Erster Prototyp (MVP):** KW 20 (16.5.-18.5.) / KW 21 (23.5.-25.5.)
* **Softwareprojektabgabe:** Ende Juni 2022 / Anfang Juli 2022
