# Gesundheitswesen

**Autor:** Malte Theodor Kanders


![THEME](media/theme_pic.jpg)

## Überblick

- Textuelle Beschreibung der Anwendungsdomäne
  - Soll dem Bürger helfen die richtige Anlaufstelle für gesundheitliche Fragen
  zu finden.
  - Soll eine Sammelstelle für Relevante Daten sein, bspw. Notfallkontakte
  - Soll von Personen im Gesundheitssystem gefüllt werden. Diese können
  sich und ihr Angebot vorstellen.


## Funktionale Anforderungen

* Definition der Akteure
  - Bürger die nach Informationen/Kontaktmöglichkeiten suchen
  - Ärzte/Apotheken/Krankenhäuser/Therapeuten die sich vorstellen und eine Kontaktstelle
  bieten


  Use Cases des Microservices:
  ![USE_CASE](media/use_case_health.png)

  Akteure:
    * Bürger
    * Gesundheitsexperten:
      * Apotheken
      * Krankenhäuser
      * Ärzte
      * Heilerzieungs....   

## Anforderungen im Detail


| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Benutzer | die Suche nutzen | nicht selber Suchen muss| Suche gibt brauchbare Ergebnisse |
| Benutzer | eine übersichtliche Seite | ich schnell finde was ich suche | wenig aber funktionale Anwendungen |
| Benutzer | einfach rumgucken können | ich vielleicht finde was ich nicht gesucht habe | Auflistung verschiedener Angebote |
| Benutzer | News sehen die relevanz haben können | ich über wichtiges Informiert bin | kleine News die Interessant sein können angezeigt bekommen |
| Benutzer | eine Kontaktschnittstelle haben | ich um persöhnliche Hilfe bitten kann | Funktionierende Kontaktschnittstelle |
| Benutzer | eine kurze grobe Übersicht relevanter Bereiche | ich einen Oberflächlichen EIndruck gewinnen kann | Auflistung mehrerer Kategorien (Optional) |
| Benutzer | sehen was ein Vertreter eines Gesundheitsvertreters anbietet | ich den richtigen Kontakt finden kann | Eine Komponente mit Stichwortartiger Beschreibung des Angebots |
| Gesundheitsvertreter | meine Angebote präsentieren | ich den Menschen meine Hilfe anbieten kann | Eine Komponente mit Stichwortartiger Beschreibung des Angebots |
| Benutzer | einen ersten Eindruck des jeweiligen Anbieters gewinnen | damit ich mich vertraut fühle | Ein kurzes Tagebuch / Curriculum Vitae |
| Gesundheitsvertreter | mich präsentieren | sich Patienten mir anvertrauen | Ein kurzes Tagebuch / Curriculum Vitae eintragen können |
| Gesundheitsvertreter | mein Team präsentieren lassen | sich auch mein Team präsentieren kann | Ein kurzes Profil eines Teammitglieds erstellen können |
| Benutzer | einen Termin online buchen könnnen | ich selbstbestimmt den Tag und die Uhrzeit bestimmen kann | einen Kalender mit auswählbaren Terminen |
| Gesundheitsvertreter | einen Terminkalender anbieten | mein Team mehr Zeit für wichtigeres hat | einen Kalender mit auswählbaren Terminen |
| Benutzer / Gesundheitsvertreter | Öffnungszeiten sichten können | diese leicht zugänglich sind | eine Zeitleiste mit Öffnungszeiten |
| Benutzer | möchte ich eine kurze News seite | ich zu aktuellen Themen benachrichtigt werden kann | Ein paar News auf einer Seite |
| Benutzer | möchte ich eine Seite mit den wichtigsten Informationen | ich Notdienste oder Notfallansprechpartner sofort finden kann | Eine Auflistung bestimmter Notfallansprechpartner |
| Benutzer | einen ersten Eindruck des jeweiligen Anbieters gewinnen | damit ich mich vertraut fühle | Ein kurzes Tagebuch / Curriculum Vitae |


## Graphische Benutzerschnittstelle

  #### Startseite/Home:

  ![HOME](media/mock_home.png)

  #### Über uns/Impressum/Hilfe
  ![ABOUT US](media/mock_about_us.png)

  #### Einzelner Service
  ![SINGLE SERVICE](media/mock_single_service.png)

  #### Kategorie/Notfallkontakt
  ![CATEGORY/EMERGENCY](media/mock_categorys_emergency.png)

  #### Aktivitätsdiagramm
  [ACTIVITY_DIAGRAMM](media/mock_activity_diagramm.png)


## Datenmodell

Vorläufige Skizze:

![ER](media/er_health_system.png)

(## Abläufe

- Aktivitätsdiagramm für den Ablauf sämtlicher Use Cases
- Aktivitätsdiagramme für relevante Use Cases
- Aktivitätsdiagramm mit Swimlanes sind in der Regel hilfreich
  für die Darstellung der Interaktion von Akteuren der Use Cases / User Stories
- Abläufe der Kommunikation von Rechnerknoten (z.B. Client/Server)
  in einem Sequenz- oder Aktivitätsdiagramm darstellen
- Modellieren Sie des weiteren die Diagramme, die für das (eigene) Verständnis des
  Softwaresystems hilfreich sind.
)

## Schnittstellen

[Api Draft](media/api_draft.pdf)
* Abhängigkeiten: Liste mit Kommunikationsabhängigkeiten zu anderen Microservices


### URL

http://smart.city/gesundheitssystem/

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
    * KTor
  * Logik-Schicht
    * Kotlin/JVM
  * Persistenz-Schicht
    * PostgreSQL

* Client
  * View-Schicht
    * KVison(React)
  * Logik-Schicht
    * Kotlin/JS
  * Kommunikation-Schicht
    * KTor/KVision


##### FullStack WebAPP in der Gesamtübersicht:

![FULLSTACK](media/sw_fullstack.png)

##### Model UML:
Hier sollen alle Klassen die wie eine Daten Klasse operieren verlagert werden. So soll doppeltes schreiben und der Vorteil der durchgängigen Benutzung einer Sprache genutzt werden. Ebenso werden die Skripte zum erstellen der passenden Datenbank Tabellen abgelegt.
![MODEL](media/sw_model.PNG)

##### Backend UML:
![BACKEND](media/sw_backend.PNG)

##### Frontend UML
Nur kurze Idee, denn da noch kein Framework für das Frontend festgelegt wurde(KVision vs React) kann nicht genau die vorgehensweise bestimmt werden.
Erst muss über beide mehr Erfahrung gesammelt werden, KVision bisher preferiert da es ohne, oder fast ohne CSS und HTML auskommt.
![FRONTEND](media/sw_frontend.PNG)

### Fehlerbehandlung

* 200 -> OK
* 204 -> No Content
* 400 -> Bad Request *beispiel wäre, die Anfrage enthielt irgendwelche komischen nicht erwünschten zusätze*
* 403 -> Permission Denied
* 409 -> Conflict *beispielhaft: Zweimal die gleiche ID beim erstellen oder irgendwas als Unique gekennzeichnetes doppelt einfügen wollen.*
* 422 -> Unprocessable Entity *beispielhaft: Sehr wahrscheinliche eine kaputte und oder falsch formatierte JSON*
* default -> unexpected Error

( ### Validierung

* Relevante (Integrations)-Testfälle, die aus den Use Cases abgeleitet werden können
* Testfälle für
  - Datenmodell
  - API
  - User Interface
* Fokussieren Sie mehr auf Integrationstestfälle als auf Unittests
* Es bietet sich an, die IDs der Use Cases / User Stories mit den Testfällen zu verbinden,
  so dass erkennbar ist, ob Sie alle Use Cases getestet haben.)

### Verwendete Technologien

* Frontend
  * KVison/React
* Backend
  * KTor
* Datenbank
  * PostgreSQL
