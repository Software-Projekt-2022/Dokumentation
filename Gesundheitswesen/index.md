# Gesundheitswesen

**Autor:** Malte Theodor Kanders


## Überblick

- Textuelle Beschreibung der Anwendungsdomäne
  - Soll dem Bürger helfen die richtige Anlaufstelle für gesundheitliche Fragen
  zu finden.
  - Soll eine Sammelstelle für Relevante Daten sein, bspw. Notfallkontakte
  - Soll von Personen im Gesundheitssystem gefüllt werden. Diese können
  sich und ihr Angebot vorstellen.
- Konzeptionelles Analyseklassendiagramm (logische Darstellung der Konzepte der Anwendungsdomäne)


## Funktionale Anforderungen

* Definition der Akteure
  - Bürger die nach Informationen/Kontaktmöglichkeiten suchen
  - Ärzte/Apotheken/Krankenhäuser/Therapeuten die sich vorstellen und eine Kontaktstelle
  bieten
* Use-Case Diagramme
* Strukturierung der Diagramme in funktionale Gruppen
* Akteure sowie andere Begriffe der implementierten Fachdomäne definieren
* Begriffe konsistent in der Spezifikation verwenden
* Begriffe im Glossar darstellen

## Anforderungen im Detail

**Screen 1**

| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Benutzer | die Suche nutzen | nicht selber Suchen muss| Suche gibt brauchbare Ergebnisse |
| Benutzer | eine übersichtliche Seite | ich schnell finde was ich suche | wenig aber funktionale Anwendungen |
| Benutzer | einfach rumgucken können | ich vielleicht finde was ich nicht gesucht habe | Auflistung verschiedener Angebote |
| Benutzer | News sehen die relevanz haben können | ich über wichtiges Informiert bin | kleine News die Interessant sein können angezeigt bekommen |
| Benutzer | eine Kontaktschnittstelle haben | ich um persöhnliche Hilfe bitten kann | Funktionierende Kontaktschnittstelle |
| Benutzer | eine kurze grobe Übersicht relevanter Bereiche | ich einen Oberflächlichen EIndruck gewinnen kann | Auflistung mehrerer Kategorien (Optional) |


**Screen 2**
| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Benutzer | sehen was ein Vertreter eines Gesundheitsvertreters anbietet | ich den richtigen Kontakt finden kann | Eine Komponente mit Stichwortartiger Beschreibung des Angebots |
| Gesundheitsvertreter | meine Angebote präsentieren | ich den Menschen meine Hilfe anbieten kann | Eine Komponente mit Stichwortartiger Beschreibung des Angebots |
| Benutzer | einen ersten Eindruck des jeweiligen Anbieters gewinnen | damit ich mich vertraut fühle | Ein kurzes Tagebuch / Curriculum Vitae |
| Gesundheitsvertreter | mich präsentieren | sich Patienten mir anvertrauen | Ein kurzes Tagebuch / Curriculum Vitae eintragen können |
| Gesundheitsvertreter | mein Team präsentieren lassen | sich auch mein Team präsentieren kann | Ein kurzes Profil eines Teammitglieds erstellen können |
| Benutzer | einen Termin online buchen könnnen | ich selbstbestimmt den Tag und die Uhrzeit bestimmen kann | einen Kalender mit auswählbaren Terminen |
| Gesundheitsvertreter | einen Terminkalender anbieten | mein Team mehr Zeit für wichtigeres hat | einen Kalender mit auswählbaren Terminen |
| Benutzer / Gesundheitsvertreter | Öffnungszeiten sichten können | diese leicht zugänglich sind | eine Zeitleiste mit Öffnungszeiten |

**Screen 3**
| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Benutzer | möchte ich eine kurze News seite | ich zu aktuellen Themen benachrichtigt werden kann | Ein paar News auf einer Seite |
| Benutzer | möchte ich eine Seite mit den wichtigsten Informationen | ich Notdienste oder Notfallansprechpartner sofort finden kann | Eine Auflistung bestimmter Notfallansprechpartner |
| Benutzer | einen ersten Eindruck des jeweiligen Anbieters gewinnen | damit ich mich vertraut fühle | Ein kurzes Tagebuch / Curriculum Vitae |


## Graphische Benutzerschnittstelle

  #### Startseite/Home: 
  
  ![HOME](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/Home.png)
  
  #### Über uns/Impressum/Hilfe
  ![ABOUT US](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/AboutUs.png)
  
  #### Einzelner Service
  ![SINGLE SERVICE](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/Single%20Service.png)
  
  #### Kategorie/Notfallkontakt
  ![CATEGORY/EMERGENCY](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/KategorienUndNotfallkontakte.PNG)
  
  #### Aktivitätsdiagramm (Kompliziertes Erscheinungsbild, aber viele Kategorien befinden sich auf ähnlichen Screens, beispiel: Home Button immer oben links führt immer zum Home -> 4 Pfeile)
  [ACTIVITY_DIAGRAMM](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/Aktivit%C3%A4tsdiagramm.png)
  

## Datenmodell

Vorläufige Skizze: 

![ER](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/media/ER_Diagramm.PNG)

## Abläufe

- Aktivitätsdiagramm für den Ablauf sämtlicher Use Cases
- Aktivitätsdiagramme für relevante Use Cases
- Aktivitätsdiagramm mit Swimlanes sind in der Regel hilfreich
  für die Darstellung der Interaktion von Akteuren der Use Cases / User Stories
- Abläufe der Kommunikation von Rechnerknoten (z.B. Client/Server)
  in einem Sequenz- oder Aktivitätsdiagramm darstellen
- Modellieren Sie des weiteren die Diagramme, die für das (eigene) Verständnis des
  Softwaresystems hilfreich sind.


## Schnittstellen

[Api Draft](https://github.com/Software-Projekt-2022/Dokumentation/blob/Unterseite-Gesundheitswesen/Gesundheitswesen/CyberCity%20API%20Draft.pdf)
* Abhängigkeiten: Liste mit Kommunikationsabhängigkeiten zu anderen Microservices


### URL

http://smart.city/microservices/wealthsystem/

### Commands / Events ?

| **Name** | **Parameter** | **Resultat** |
| :------ | :----- | :------ |
| createHelthExpert() | int x_id, timestamp x_date, x_name string, x_title string | int id |
| createCrewMember() | int crew_id, timestamp crew_date, crew_name string | int id | 
| removeHealthExpert() | int id | int id |
| removeCrewMember | int id | int id |
| createBreakingNews | int n_id, string message | int id |



## Technische Umsetzung


### Softwarearchitektur

- Darstellung von Softwarebausteinen (Module, Schichten, Komponenten)


* Server
  * Web-Schicht
  * Logik-Schicht
    * Kotlin/JVM
  * Persistenz-Schicht
    * MySQL 

* Client
  * View-Schicht
    * Kotlin Framework
  * Logik-Schicht
    * Kotlin/JS
  * Kommunikation-Schicht
    * Retrofit?


### Entwurf

- Detaillierte UML-Diagramme für relevante Softwarebausteine

### Fehlerbehandlung

* Mögliche Fehler / Exceptions auflisten
* Fehlercodes / IDs sind hilfreich
* Nicht nur Fehler technischer Art ("Datenbankserver nicht erreichbar") definieren, sondern auch fachliche Fehler wie "Kunde nicht gefunden", "Nachricht wurde bereits gelöscht" o.ä. sind relevant.

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
  * Kotlin/JVM Framework: KVision?
  * Retrofit?
* Backend
  * Kotlin 
  * Spring Boot / Ktor
* Datenbank
  * MySql 
