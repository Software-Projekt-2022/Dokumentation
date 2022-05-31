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

## 19.04.2022 14:30 - 17:00
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
* SM und PO müssen mehr auf Microservice Ebene die Issues schreiben. So können wir einen gerechten Arbeitsaufwand pro Woche gewährleisten.
* Fragerunde mit den Software Engineers in der wir deren Aufgaben für Sprint 2 besprechen und einteilen.

## 26.04.2022 14:30 - 16:00
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
* Hat das Team fragen?
  * Der DevOps Engineer würde gerne von jedem Mitglied Deployment informationen haben
    * Wir haben einen Discord Thread erstellt in dem jeder seine Informationen rein schreibt
    * Informationen werden schnell benötigt damit die Engineers möglichst bald in die Entwicklung starten können
* Wie werden Pull Requests im Team durchgeführt
* Code Review Kriterien
  * Funktionalität
    * Testfälle laufen durch
  * Dokumentation
    * Muss für einen fremden lesbar sein 
  * Code Qualität
    * Aussagekräftige Variablennamen
    * kein auskommentierter Code
    * Formatierung
    * einheitliche Sprache
    * Code Kommentare, Commits und Variblennamen auf Englisch
    * Logische Aufteilungen, gute Struktur
 * Frontend auf Deutsch
 * Sprint nachbesprechung
   * Sollen wir den Sprint verlängern?
     * Verlängern
     * Zu viele Aufgabne offen um sie in die nächste Woche zu übernehmen
 * Einheitliche Schriftfarbe und Fonts beachten
 * der Name ist "CyberCity" und alle anderen Varianten sollten angepasst werden 
 * Weitere Fragen vom Team
   * Eine Datenbank im Container?
   * Mehr als ein Container pro Repo?
   * Was spricht für eine Trennung von Frontend und Backend Container
   * Umgang mit Umgebungsvariablen?
 * Authentifizierung
   * Wie können die anderen Services die Authentifizierung nutzen?
   * Beim login in der Landing Page erhält man einen Token, dieser wird dann von den anderen MS gegriffen und zur kann zur Validierung zum AuthMS geschickt werden
   * Fragen zu den Token?
 * Events
   * JSON Schema im nächsten Sprint erstellt

## 03.05.2022 14:30 - 15:30
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
* Herr Brunsmann gibt eine kleinere Agenda für heute vor
* Zuerst stellt jeder seinen Fortschritt vor
  * Jonas
    * DB Statements fertig, Verknüpfungen in Node.js fertig
    * HTML Pages existieren
    * lokal läuft es
    * Deployment/Containerisierung fehlt
  * Toni
    * API funktioniert
    * HTML existiert, für 48h kann Wetter/Pollen angezeigt werden
    * Layout muss noch erstellt werden
    * Deployment/Containerisierung fehlt
  * Malte
    * Grundgesrüst (Visueller Part und DB) steht
    * Datenbankschema fehlt noch
    * Natives React Problem behoben, mit KVision umgesetzt
    * Deployment/Containerisierung fehlt
  * Jason
    * Login/Registrierung, Verifizierung per Email funktioniert
    * Probleme mit PostgreSQL, Zugriff über Kommandozeile funktioniert nicht
    * Deployment/Containerisierung fehlt
  * Clemens
    * DB fertig
    * API zum großteil fertig
    * Website ist grafisch verfügbar, aber wenig funktionen
    * Container läuft
    * Deployment fehlt
  * Mattis
    * Website statisch fertig, keine funktion
    * API großteils fertig
    * DB nicht angefangen
    * Docker läuft für Website auslieferung
    * Deployment fehlt
  * Leon
    * Traefik Grundkonfiguration funktioniert
    * RabbitMQ funktioniert, wird erfolgreich Deployed, vorgegebene JSON wird geladen und setup Script wird ausgeführt
    * Erklärt wie er die ganzen Container erstellen will
  * Andreas
    * Fehlerbehandlung RabbitMQ, neuer Event-Type
    * Event umbenannt, Beispiel Code für RabbitMQ
    * Validierung der Events noch nicht vorhanden
    * JSON Schema steht noch aus
  * Tim
    * Landing Page Docker konfiguration wollte erst nicht
    * Landing Page läuft im groben
    * Verlinkungen zu den MS noch testen und dann eventuell anpassen
    * Meldungs/Nachrichtenansicht über Zugriff auf den Meldungsbus noch ausstehend
  * Mark 
    * Meetingsplanung für den 03.05.2022
    * Individuelle Gedanken zu jedem Repo, jeder Person und der Scrum Arbeitsweise
    * Arbeitsstandüberprüfung der Microservices
* Dann reden wir über Hindernisse/Probleme auf technischer und menschlicher ebene
* Weiteres vorgehen für den nächsten Sprint
* Dann erstellen wir einen Termin für das MVP
  * Vorschlag: 24.05.2022
  * Vorschlag wurde angenommen
* Fragen an Herrn Brunsmann
  * Es gab keine Fragen
* Mark übernimmt Organisationsleitung
* Bitte nicht die PRs selber mergen ohne, dass diese approved wurden
* PR workflow beschrieben
* wo bleibt HTTPS? Mit zertifikaten starten dauert zu lange
* Es sollen auch in der Zukunft keine CORS fehler auftreten deswegen schnell HTTPS einstellen
* Pull Requests am Ende von einem Sprint
* versuch Jasons Push Probleme zu lösen
* Container Aufgabe wird noch eine Woche weiter geschoben, diesmal aber priorisiert
* Unternehmensregister, welche User Story kommt als nächstes
* der Software Architekt hat bereits zwischen Meeting Vorbereitung und Meeting alle offenen PRs bearbeitet und muss jetzt auf die nächsten warten
* Fragen?
  * Issues werden nur vom Product Owner oder Scrum Master geschlossen
* kleinere Diskussion über den nächsten Sprint

## 10.05.2022 14:30 - 16:15 (Online-Meeting wegen Corona Fällen)
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Jason Piper | Software Engineer |
| Mattis Fieseler | Software Engineer |
| Toni Schnittger | Software Engineer |
| später erschienen |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Clemens Maas | Software Engineer |
| krankheitsbedingt ausgefallen |
| Jonas vom Braucke | Software Engineer |

### Themen
* Das heutige Meeting wird online stattfinden, da es mehrere Corona Fälle im Team gibt
* Sprint 2 nachbesprechung
* PR Tipps und Tricks (close, etc.)
* Pull Requests überprüfen
* **wichtige Infos zu PRs: Immer am Ende eines Sprints von allen Development Branches in main, schließt die Issues die in der Woche bearbeitet wurden mit "close #issueid"**
* wie weit sind die Software Engineers diese Woche gekommen
  * Mattis:
    * Frage zum Datenmodell, ist aber fertig
    * Backend fertiggestellt
    * anstehende Events
    * eine Issue wird in die nächste Woche übernommen
  * Jason:
    * Dockerfile probiert, erst Probleme dann Kommilitonen gefragt
    * mit DB verknüpfen eventuell fertig, aber email senden fehlerhaft und stoppt den server
    * Passwort vergessen/reset noch nicht angegangen
  * Toni:
    * Wasserstand API fertig und dargestellt
    * Design verbessert
    * unser Design eingebaut (font/farben)
    * weitere Gedanken zum Design
  * Tim:
    * LandingPage weiter bearbeitet
    * Services werden noch nicht so schön dargestellt
    * Dockerfile läuft soweit
   * Andreas:
     * JSON Schemas für die Events sind fertig
     * befinden sich im zugehörigen Repo im Ordner Schemas
     * Pull Requests reviewed
     * RabbitMQ eigentlich fertig
     * Hauptaufgabe ab jetzt die Pull Requests
   * Leon:
     * Muss den Fehler in Event_service Deployment noch beheben -> findet Skript nicht
     * Lokal ausführen von Event_Service Deployment funktioniert
     * fast alle Dockerfiles fertig, DB in den selben Container macht Probleme
     * ein Dockerfile schwieriger wegen Payara
   * Malte:
     * kein allzu größerer Fortschritt
     * Dockerfile versucht zu schreiben
     * versuch das Dockerimage fertigzustellen, da gibt es noch Probleme mit dem Frontend
     * Absprache mit Leon zum Dockerimage
   * Clemens:
     * Einbindung JS ist fast fertig
     * Bewerbungsmanager: Bewerbungen schreiben, sehen funktioniert. Da login durch Authentifizierung noch fehlt geht bewerben über Profile nicht
     * warten bis Authentifizierung fertiggestellt und deployed ist
     * Issues sind alle Ready for Review
     * hat eigene Todos im Repo geschrieben um die logischen nächsten Schritte darzustellen
 * RabbitMQ läuft auf http://cyber-city.systems:15672/
 * Dockerfile in Event_Service fertig, aber Github Actions läuft nicht durch
   * Scheinbar versucht Github das Dockerimage zu bauen und dann zu DigitalOcean zu senden aber das funktioniert noch nicht
   * Dockerfile führt Skript aus
 * Deployment
 * Leon führt noch ein persönliches Meeting um ein Problem mit den Dockerfiles zu beheben
 * Müssen DB und Microservice wirklich im selben Container laufen? -> Wir sagen weiterhin "ja", obwohl DB als eigener Container einfacher wäre
 * PR vom Gesundheitswesen von dev in main erstellt, letzte Woche falscher PR
 * An alle: PR für diesen Sprint stellen um die Changes von allen Entwicklungsbranches in den main zu mergen!
 * Fragen?
 * Alle Elemente von Sprint 3 die nur auf Todo standen wurden in Sprint 4 übernommen.
 * Alle Issues von Jonas werden übernommen, da er Krankheitsbedingt ein paar Tage ausfiel und diese nicht fertig bearbeiten konnte. Da er schon an den Issues gearbeitet hat bekommt er zusätzlich noch weitere.

## 17.05.2022 14:30 - 16:00
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Mattis Fieseler | Software Engineer |
| Clemens Maas | Software Engineer |
| Malte Kanders | Software Engineer |
| krankheitsbedingt ausgefallen |
| Jonas vom Braucke | Software Engineer |
| Toni Schnittger | Software Engineer |
| nicht vor Ort |
| Jason Piper | Software Engineer |

### Themen
* Toni und Jonas sind beide krank, haben sich aber abgemeldet
* Jason ist nicht vor Ort und kann deswegen auch nicht teilnehmen
* Was haben die Mitglieder diese Woche gemacht
  * Malte
    * Kotlin Projekt verworfen
    * Web Applikation auf Javascript umgestellt
    * Dockerfile dafür fertig
    * Wie siehts aus mit Issue 4 und 5? Verschieben auf nächste Woche weil nach der Umstellung nicht so viel Zeit war
  * Mattis
    * Seiten für Vereine und Chats fertiggestellt
    * Bootstrap selbst recherche
    * Issue 4 ist fertig
    * Issue 5 ist Backendseitig implementiert
    * Issue 6 ist noch auf Todo, muss dann mitgenommen werden
    * Schau dir bitte den Kommentar zu deinem Pull Request an
  * Clemens
    * Testen der bisherigen Anwendung
    * wartet auf Authenifzierung Deployment sonst soweit fertig
  * Leon
    * Dockerfiles fast fertig, 2 Kompilieren nicht
    * Git Workflows fertig
    * 2 Repositories schlagen beim Dockerfile fehlt
  * Andreas
    * Alle Pull Requests angeschaut und eventuell Kommentare geschrieben
    * die Pull Requests durchgeführt
  * Tim
    * Landingpage im Design weiter angepasst/verbessert
    * auf andere Module konzentriert
* Leon fügt an, dass die jar die im Microservice vom Gesundheitswesen generiert wird von gradle nicht ausgeführt werden kann
* kleinere Besprechung dieses Problem zu resolven
* kleinere nebenbesprechung über Benachrichtigungen durch Pull Requests von Mattis und Andreas
* Gruppenbildung um verschiedene Problemstellen zu lösen
* Wann kommen die Dockerfiles und das Deployment? Jeder der Services benötigt jetzt die Authentifizierung und bis zum MVP **müssen** alle Services Deployed sein.
* warum läuft die Action nicht durch? Das liegt an Docker compose, der Container wird aktuell noch falsch gebaut
* Wie viele Container hat jetzt jeder Service? Die meisten haben einen Container, nur das Unternehmensregister hat zwei
* Wo sind die Websites von DigitalOcean? 
  * Das Problem war unbekannt
  * Das liegt an dem Docker Compose von RabbitMQ
  * wenn RabbitMQ Problem resolved ist sollten alle Websites wieder verfügbar sein
* Leon soll bitte heute Abend mit Jason in Kontakt treten damit die Authentifizierung möglichst schnell läuft
* Wenn das Deployment nicht funktioniert bis zum Wochenende wird online eine Krisensitzung gehalten
* Dockerfiles müssen jetzt einzeln auf jedem Repo durchgeschaut werden und dann werden die Issues auf done geschoben
  * Zuständiger: Andreas
  * soll bei Problemen Leon direkt schreiben
* Wie gehen wir mit den Relikten aus Sprint 4 um?
  * Sprint 4 wird verlängert, da die meisten Issues nicht fertig sind und es auch viele krankheitsbedingte Ausfälle die Woche gab
  * Sprint 4 wird ergänzt um die Issues die für den MVP wichtig sind
* nach dem MVP werden die Sprints nicht mehr standardmäßig 7 Tage, sonder 14 Tage dauern
* MVP Ziele definieren in einem anderen Dokument, Link hier: https://software-projekt-2022.github.io/Dokumentation/#/_einleitung/mvp

## 23.05.2022 15:00 - 16:30 (Online-Meeting)
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Mattis Fieseler | Software Engineer |
| Clemens Maas | Software Engineer |
| Malte Kanders | Software Engineer |
| Jonas vom Braucke | Software Engineer |
| Toni Schnittger | Software Engineer |
| Jason Piper | Software Engineer |

### Themen
* Was haben die Software Engineers die Woche gemacht, was wird noch gemacht für den MVP?
* Andreas:
  * Pull Requests bearbeitet
* Leon:
  * Deployment aller Microservices vorbereitet
  * RabbitMQ wieder Deployed
* Jonas:
  * SQL Statements angepasst für das Deployment, secondary Keys machten Probleme
  * die ersten beiden Seiten fast fertig, push auf git ausstehend
  * Sobald DB Connect im Deployment funktioniert sollte Deployment vom Verkehr Microservice durchlaufen
  * RabbitMQ Schnittstelle implementiert
* Toni:
  * Falsche Wochentage gefixed
  * Event senden vorbereitet
  * RabbitMQ Schnittstelle vorbereitet
  * Hardcoded Beispieldaten aus HTML entfernen
* Clemens:
  * Mithilfe beim Deployment von seinem Microservice
  * Probleme beim Deployment durch/bei Springboot .jar erstellung
  * Frontend erweitert
* Mattis:
  * Backend für Deployment gefixed
  * Backend ergänzungen
  * Frontend für Deployment gefixed, sollte starten können
  * Frontend Layout verbessert
* Jason:
  * hat beschlossen SWP nicht weiter zu machen
  * Tabellen werden nicht erstellt, sollten Tabellen erstellt werden sollte Deployment funktionieren
    * Lösungsansatz: E-Mail Service entfernen
    * Sonst Fehlermeldungen in Spring anschauen
* Malte:
  * Frontend verschiedene Routen zwischen denen gewechselt werden kann
  * Frontend und Backend arbeiten zusammen
  * Interne Schnittstellen alle definiert
  * Erste Frontend Seiten verfügbar
* Einschätzung des DevOps Engineer zum Deployment Status: Unbekannt, man kann die Probleme nicht vorher abschätzen
* Nochmal über alle MVP Ziele drüber schauen und nach Wichtigkeit sortieren, den Mitgliedern mitgeben was noch zu machen ist
* Alle Software Engineers sollen noch Pull Requests stellen um ihre Fortschritte von Dev in Main zu pushen.
* Problem Solving im gesamten Team
* Nochmal Kanban Verläufe ansprechen:
  * Dran denken den PR zu stellen
  * Dran denken Issues weiter zu schieben
  * Transparenz sehr wichtig, gerne öfter im Discord schreiben und andere informieren

## 24.05.2022 MVP Vorstellung 14:30 - 16:15
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Mattis Fieseler | Software Engineer |
| Clemens Maas | Software Engineer |
| Jonas vom Braucke | Software Engineer |
| Toni Schnittger | Software Engineer |
| krankheitsbedingt nicht vor Ort |
| Malte Kanders | Software Engineer |

### Themen
* Herr Brunsmann auf den neuesten Stand gebracht:
  * Malte fällt Krankeheitsbedingt aus
  * Jason hat mit Softwareprojekt aufgehört
* MVP wird vorgestellt in folgender Reihenfolge:
  * Tim und die Landingpage
    * Zuerst die Landingpage an sich
    * dann Codeausschnitte
  * Malte und das Gesundheitssystem
    * Zuerst die Seite
    * dann Codeausschnitte auf nachfrage durch Herrn Brunsmann
    * Zeigt den Deployment Prozess
  * Mattis und die Kulturseite
    * Zuerst die Seite
    * dann Codeausschnitte vom Glassfish Backend
    * Codeausschnitte der Eventanbindung
  * Clemens und das Unternehmensregister
    * Zuerst die API Routen über Swagger Dokumentation
    * dann die Seite
    * source Code vom Frontend
    * Erklärung zu Next.JS
  * Toni und die Umweltseite
    * Zuerst die Website
    * dann Source Code vom Frontend
    * Source Code für Events im Backend
  * Jonas und die Verkehrseite
    * Zuerst das Frontend
    * dann Source Code vom Frontend
    * Source Code vom Backend
  * Andreas und RabbitMQ
    * Zeigt die Frontend Seite von RabbitMQ
    * Zeigt an Beispielen den Umfang von RabbitMQ
    * Dann anhand vom Source Code wie RabbitMQ aufgebaut ist
    * Beschreibt einmal wie er Code Reviews durchführt
  * Leon zeigt das Deployment
    * Docker Compose file
    * Identifikation der Fehler, zeigt Notizen dazu (Excel)
* Jeder soll Tests schreiben
* Projekt wirkt sehr unintegriert, da noch die Kommunikation zwischen den Services fehlt
* Wie gehen wir weiter vor, wer übernimmt Authentifizierung? Andreas übernimmt den Service, Scrum Master und Prduct Owner unterstützen dabei
* Authentifizierung ist ein wichtiges Standbein für das ganze Projekt und muss bis zum Ende funktionieren.
* zum MVP waren die wichtigsten Grundfunktionen vorhanden
* es gibt trotzdem noch viele Baustellen bis zur Abgabe
* Technische Heterogenität ist sehr gut, herausfordernd für die CI/CD Pipeline
* am 07.06.2022 Terminfindung für die Abgabe
* Wie funktioniert Authentifizierung, wer übernimmt es? Kleinere Diskussion
* Wie kann man die User in den Mircroservice Datenbanken erweitern? Kleinere Diskussion
* Nehmen wir JWT Token für die Authentifizierung? Vorteile und Nachteile Diskussion
* Weitere Vorschläge: Passport.js
* Wie sende ich Zeitbasierte Events? Vorschläge:
  * Timer und Callback auf das senden des Events
  * Eventuell beim Login von einem User
  * Nur beim Page Aufruf

## 31.05.2022 Zwischenstandsbesprechung 14:30 🕝 - 15:30 🕞
### Teilnehmer
| Teilnehmer | Rolle |
| - | - |
| Mark Mödeker | Scrum Master |
| Tim Bollmeyer | Product Owner |
| Andreas Wegner | Software Architekt |
| Leon Stümpeley | DevOps Engineer |
| Malte Kanders | Software Engineer |
| Mattis Fieseler | Software Engineer |
| Jonas vom Braucke | Software Engineer |
| Toni Schnittger | Software Engineer |
| krankheitsbedingt ausgefallen |
| Clemens Maas | Software Engineer |

### Themen
* Nachbesprechung MVP
* wie weit sind die Software Engineers jetzt bei der Hälfte des Sprints?
  * Mattis
    * Backendarbeiten
    * Datenbankstruktur geändert, Place auf mehrere Tabellen und mit Joins verknüpft
    * Beispieldaten geschrieben
    * Frontend API Pfade hinterlegt
  * Jonas
    * ViewJS auseinandergesetzt
    * CSS überarbeitet
    * Einbindung in RabbitMQ fast vollständig
    * Rest Schnittstelle angefangen
  * Leon
    * Unternehmensregister Frontend läuft
    * Alle Services die nicht laufen angeschaut
  * Andreas
    * Authentifizierungs Service vollständig neu aufgebaut
    * Authentifizierung selber deployed damit die Software Engineers es nutzen können https://lulon.ddns.net
    * Soll noch die Dokumentation für die Authentifizierung anpassen
* Tim soll seinen Link für das Unternehmensregister ändern auf die neue Adresse und Clemens kann aufhören seine Seite zu hosten
* Andreas präsentiert seinen Authentifizierungs-Service
  * Präsentation Swagger Dokumentation
  * API Routen in Postman zeigen
* Q&A zu der Authentifizierung
  * Wie wird die Verschlüsselung umgesetzt?
  * Wie lange ist das JWT gültig?
  * Wo ist das aktuelle Repo angelegt, wie kommt es in die Organisation?
  * ist das Dockerfile so vernünftig?
  * Wofür ist der Public Key beim JWT?
* Neue Events:
  * Jedes mal wenn sich ein User registriert schickt die Authentifizierung ein Event mit allen Daten außer dem Passwort an die anderen Services. So können die anderen MS die User auch bei sich angelegen. 
  * Wenn ein User seinen Account löscht wird das auch gesendet.
* E-Mail Authentifizierung? 
  * Diskussion zur Email Authentifizierung
