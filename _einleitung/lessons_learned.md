# Lessons Learned

Auf dieser Seite hat jeder aus dem Team einmal seine persönlichen Lessons Learned niedergeschrieben.

## Mark Mödeker - Scrum Master

Für mich war es anfangs schwierig meine Rolle im Projekt für mich zu definieren. Da ich als Scrum Master eine leitende Position im Team hatte
fand ich es schwierig, wie ich mit den restlichen Mitgliedern kommunizieren sollte, da ich nicht wie jemand auftreten wollte der nur Aufgaben 
verteilt, aber nichts macht. Vor allem weil wir als Studenten alle gleichgestellt sind und nur für das Projekt die Rollen annehmen sollten.
Ich habe dieses Problem dann so bewältigt, dass ich auf unserem Kommunikationsserver mehrere Tutorials verfasst habe für unter anderem 
den Git Workflow, Pull Requests oder den Login Prozess und, dass ich versucht habe das Team zu koordinieren, indem ich geschaut habe in 
welchen Microservices ähnliche Techniken verwendet werden, damit sich die jeweiligen Teammitglieder dann ein wenig gegenseitig helfen können.

Es war das erste Mal, dass ich eine leitende Position in einem Softwareprojekt angenommen hatte und deswegen hat es erst eine kleine
Eíngewöhnungsphase gebraucht bis ich meine Rolle richtig einordnen konnte, aber ich glaube ich habe das im Endeffekt gut bewältigt.

Als Scrum Master musste ich auch regelmäßig in unserer GitHub Organisation schauen, ob alle Mitglieder die Scrum Arbeitsweise einhalten.
Da das Kanban Board auf der obersten Ebene für alle Microservices einsehbar war, war es einfach zu schauen ob die Issues regelmäßig in die richtige
Spalte geschoben werden. Schwieriger war es zu schauen ob die restlichen Schritte vom Git Workflow eingehalten wurden, da z.B. nicht auf dem
Main Branch gearbeitet werden sollte, weil dieser immer deployed wird, und deswegen nur größere Änderungen gebündelt über Pull Requests auf
den Main gepushed werden sollten. Dies wurde öfter unübersichtlich, da ich auf jedes Repository einzeln gehen musste um die oben genannten Aspekte
zu überprüfen.

Eine weitere Sache, die ich mir für zukünftige Projekte merke, ist auf jeden Fall am Anfang des Projektes den Kommunikationsweg zu definieren. Wir
hatten zwar von Anfang an einen Server, aber die meisten Nachrichten wurden eher im privaten verschickt was nicht gut für die Transparenz war.
So wusste nicht jeder, woran die anderen Mitglieder gerade sitzen und wie weit sie mit ihrer Aufgabe sind, deswegen auch die oben angesprochenen
Koordinierungsversuche. Für meine nächsten Projekte würde ich also versuchen alle zu überzeugen immer auf dem Server zu schreiben um die
Transparenz zu fördern.
 
Zusammengefasst kann man sagen, dass es als Scrum Master schwierig ist einen gesunden Mix zu finden mit den Mitgliedern auf zwischenmenschlicher
Ebene gut zurechtzukommen und trotzdem als Autoritätsperson die Aufgaben zu verteilen.

**wichtigste Lessons Learned**
- Kommunikation mehr im Team, nicht zwischen einzelnen Personen
- Nachrichten auf dem Server sollten gelesen werden
- Früher die Mitglieder an die Aufgaben erinnern
- auch zu Pull Requests hinzufügen lassen damit man eine gesammelte Übersicht auf GitHub bekommt

## Tim Bollmeyer - Product Owner

Zielsetzung unseres ***CyberCity***-Softwareprojekts war es 
die digitale Transformation von Kommunen abzubilden und ein digitales Angebot von kommunalen Diensten zu implementieren.  
Als *Product Owner* unseres Projekts stand ich dabei vor der Herausforderung, die Entwicklung der 7 individuellen Microservices zu koordinieren und auf die Erreichung dieses Projektziels hinzuwirken. 

Die Zuteilung von Aufgaben hat in meinen Augen großes Potential die individuelle Motivation aller Beteiligten zu gefährden. Um dies zu vermeiden und sicherzustellen, dass die jeweiligen Softwarengineers ihre Microservices nach ihren Vorstellungen umsetzen können, habe ich anfangs beschlossen die produkt-bezogen Issues nicht zu strikt zu gestalten. 
Eher habe ich versucht den Fortschritt des Projekts entlang der Entwicklungsschritte zu koordinieren. 
Zur Organisation und Zuteilung der Issues haben wir ein GitHub-Kanbanboard auf Ebene unserer GitHub-Organisation aufgesetzt. So wollten wir den Projektfortschritt an zentraler Stelle abbilden und visualisieren. 
Für jedes Repository habe ich dann für unsere Sprints die nächsten Issues erstellt und zusammen mit dem *Scrum Master* zugeordnet.
Im Laufe des Projekts hat sich jedoch immer wieder gezeigt, dass die Beurteilung des Projektfortschritts nur sehr schwierig möglich war.
Eine Ursache dafür ist, dass das Kanbanboard meist nur durch wiederholte Aufforderungen des *Scrum Masters* aktualisiert wurde. Außerdem klappte die Kommunikation auf dem gemeinsamen Discord-Server nicht. Viele Probleme wurden bspw. in eigenen Chats zwischen DevOps-Engineer und Softwarengineers angesprochen, nicht jedoch für alle transparent auf dem Discord-Server.

Eine weitere wichtige Lesson, die sich stark auf unser Projekt ausgewirkt hat, sind Abhängigkeiten zwischen einzelnen Produktkomponenten, sowie zur Infrastruktur. Da ist einmal unser Authentifizierungsservice und der Ausstieg eines Teammitglieds zu nennen. Aber auch das Deployment der Services führte oft zu Sätzen wie: "Lokal lief alles bei mir, in der deployten Umgebung geht nichts mehr".
CORS, falsche Pfade/Hostnamen etc. bereiteten einige Probleme und sorgten für Verzögerungen im Projektverlauf. Oftmals ging es mehr um Fehlersuche, als um tatsächliche Weiterentwicklung des Produkts.

Sollte ich in Zukunft noch einmal die Rolle eines *Product Owners* erfüllen, möchte ich möglichst früh eine konkrete und möglichst umfängliche Vision des Endprodukts entwickeln und für alle greifbar machen. Durch inkrementelle Verbesserungen des deployeten Produkts - möglichst ab einem frühen Zeitpunkt - möchte ich dann durch spezifischere Issues und häufigeres Feedback mehr auf das Produkt (und den Mehrwert der Nutzer) einwirken.
Fraglich ist jedoch, ob dies im Rahmen des Studiums (Zeitmanagement, andere Module...) entsprechend der eigenen Vorstellungen/Zielsetzung möglich ist.


Abschließend noch einmal meine Top ***Lessons Learned*** in Stichpunkten:

- sehr komplex den Entwicklungsstand von vielen (verschiedenen) Produktkomponenten im Blick zu behalten und zu koordinieren 
- Abhängigkeiten kritisch für Projekterfolg
- Kommunikation und Integration sind Grundlage für erfolgreiches Projekt


## Leon Stümpeley - DevOps Engineer
Als DevOps-Engineer war ich in diesem Projekt in einer Position, wo ich mich mit den Umständen jedes Microservices auseinandersetzen musste. Die Komplexität dessen hatte ich von Anfang an unterschätzt. Ich hatte mir für das Deployment und die automatisierten Workflows zwar schon von Anfang an ein konkretes Ziel gesetzt, dieses hat sich aber durch den Fortschritt des Projektes wiederholt an die Bedürfnisse angepasst. Das erste Mal musste ich meine Deployment-Vision anpassen, als die Softwareengineers, wider meiner Planung, verschiedene DBMS benutzen wollten. Anstatt einem zentralen Datenbankserver (von Anfang an war es der Plan, dass jeder Service eine getrennte Datenbank hat) haben wir nun verschiedene Datenbankcontainer, einen für jeden Service. Ich hatte auch erst geplant, dass die Services die Datenbank-Tabellen selbständig einrichten, aber von vielen Services habe ich dann ein SQL-Skript bekommen, mit dem ich eigenständig die Datenbank anlegen sollte, sofern sie noch nicht vorhanden ist. 

Die Services in die Docker-Images zu bauen war zum Großteil kein Problem, aber meine allgemeine Herangehensweise an das Thema war nicht optimal. Ich wollte die Docker-Images für die Services selbst erstellen, anstatt den Engineers dieses selbst zu überlassen, aber nicht alle Engineers waren damit zufrieden. So haben ein paar Engineers ihre Docker-Files selbst erstellt, wodurch sich Fehler eingeschlichen haben.
Die Zusammenarbeit mit den Engineers lief ziemlich zufriedenstellend, aber es gab doch einige Herausforderungen. Das Umstrukturieren der Services ergab sich als schwererer, als die Engineers gedacht hatten und so ist es auch zu folgendem Fall gekommen:
Bei einem unserer Meetings stellte sich beiläufig heraus, dass nicht die aktuelle Version seines Services deployed war. Stattdessen war die 2 Wochen alte Version deployed. Er hatte den Frontend Ordner verschoben, wodurch das Docker-Image nicht gebaut werden konnte. Ich habe auch leider die Benachrichtigung von GitHub Actions nicht gesehen, da ich zu dem Zeitpunkt eine Herausforderung bei einem anderen Service gelöst habe und ich zu dem Zeitpunkt eine große Anzahl an Nachrichten erhielt.

Ich habe teilweise zu viel Zeit mit einem einzelnen Service verbracht, obwohl das Problem nicht am Deployment, sondern am Service lag. Ich habe wiederholt lernen müssen, dass, obwohl der Service lokal beim Engineer liefe, einige Probleme am Service selbst liegen können, nicht am Deployment.

Zum Beispiel hatte ein Service sich auf den Localhost gebindet, anstatt auf 0.0.0.0 und ich habe viel Zeit damit verbracht, die Konfiguration des Containers und des Reverse-Proxys auf Fehler zu überprüfen. Auch habe ich am Anfang eine halbe Nacht lang einem Engineer geholfen ein SQL-Skript zu debuggen, da dieses Lokal keinen Datenbankserver aufsetzen wollte.

Sollte ich in Zukunft noch einmal als DevOps-Engineer arbeiten, habe ich nun viele Einblicke in die Konfiguration der Reverse-Proxy, der Workflows und der Deployment-Umgebung erhalten, sowie in Probleme, die an bestimmten Punkten der Planung, Ausführung und Optimierung aufkommen können und wie ich diese richtig Vermeide, Diagnostiziere und behebe.


## Andreas Wegner - Software Architekt, Software Engineer

### RabbitMQ

Zu Beginn lag der Schwerpunkt für mich darin, herauszufinden, wie man mit RabbitMQ
arbeitet und wie wir dies am besten in unser Projekt einbinden. Mein Ziel dabei, war es
die Einbindung so zu gestalten, dass jeder von uns es leicht hat, damit zu arbeiten.

Nachdem ich mich selbst mit RabbitMQ vertraut gemacht habe, war es an der Zeit,
mein Wissen an meine Teammitglieder weiterzugeben. Das war gar nicht so leicht,
da viele Menschen einen unterschiedlichen Lerntyp haben und es vermutlich deswegen manchmal
zu Missverständnissen gekommen ist.

Ich fühle mich teilweise schlecht darüber, dass ich nicht gut genug kommuniziert habe,
als ich eine bestimmte Idee mit dem Team teilen, wie wir am besten mit RabbitMQ arbeiten.
Die Idee war ein interner Server, der RabbitMQ weg abstrahiert und dadurch Fehlerquellen reduzieren sollte.
Gerade hier kam es meiner Meinung nach zu Missverständnissen.
Letztendlich weiß ich nicht, ob diese Idee wirklich besser wäre, aber ich hätte sie gerne mit dem Team ausprobiert.
Daraus lerne ich zum Beispiel, dass ich meine Erklärungen und Vorschläge besser vorbereiten sollte,
bevor ich sie dem Team vorstelle und gegebenenfalls mit Diagrammen und ähnlichem unterstütze.

### Code-Reviews

Bei den Code-Reviews war es meine Aufgabe, mir bei jedem Pull-Request die Änderungen in den Commits anzusehen
und dann den Code zu bewerten. Bewertet wird nach den von uns im Voraus bestimmten Kriterien.
Ich muss dann entscheiden, ob der Code in unser Projekt übernommen wird, oder ob vorher noch Änderungen
übernommen werden müssen.
Dabei hatte ich sofort bei den ersten Code-Reviews, die Sorge, jemals Code zu bemängeln.
Denn ich weiß, dass die Software-Engineers von uns hart arbeiten, um den Code zu schreiben
und mochte es nicht, dann noch den Code zu bemängeln.
Ich weiß, dass wir unter einem gewissen Zeitdruck arbeiten und die Software-Engineers auch Studenten sind,
die auch noch andere Arbeit haben, und nicht begeistert sind, wenn unerwarteterweise noch mehr Arbeit auf sie wartet.

Im Nachhinein denke ich, dass es gut wäre, von Anfang an zu kommunizieren, dass eingeplant werden muss,
dass nach einem Pull-Request Code noch angepasst werden muss, falls er im Code-Review bemängelt wurde, was wahrscheinlich ist.

Zusätzlich muss ich sagen, dass ich zu Beginn des Projekts deutlich mehr Zeit hatte, um Code-Reviews
zu machen, als gegen Ende des Projekts. Am Ende des Projekts war der Abstand zu den Pull-Requests teilweise so klein,
dass es sehr unrealistisch war, vernünftige Code-Reviews zu machen, vor allem wenn dann noch Code bemängelt wird,
welcher dann noch angepasst werden muss. Der Software-Engineer, der den Pull-Request gestellt hat,
arbeitet wahrscheinlich auch direkt weiter und kann nicht unbedingt zurückspringen, um die Mängel zu beheben.

Ich glaube, dieses Problem zu beheben ist ziemlich schwer, da es normal ist, dass gegen Ende eines Projekts
mehr gearbeitet wird, da der Druck erhöht wird.
Man könnte zwar einen sehr strengen Zeitplan erzwingen, aber das ist eher kontraproduktiv, da dieser dann
trotzdem nicht immer eingehalten wird und das für mehr Komplikationen sorgen könnte.

### Authentifizierungs-Microservice

Da ein Teammitgliede das Team verlassen hat, musste seine Aufgabe, den Authentifizierungs-Microservice zu programmieren,
übernommen werden. Da ich zu dem Zeitpunkt besonders motiviert war und gerade etwas mehr Zeit hatte,
habe ich freiwillig, den Authentifizierungs-Microservice neu programmiert.
Hier konnte ich noch einmal etwas für mich wiederholen, wie man ein Login-System schreibt.

### Zusammenfassung

* Bei RabbitMQ gab es einige Missverständnisse. Ich hätte Erklärungen besser vorbereiten sollen.
* Code-Reviews sollten besser geplant werden, damit es auch zeit-technisch keine Probleme gibt.

## Jonas vom Braucke - Software Engineer

## Toni Schnittger - Software Engineer
Am Anfang des Projekts hatte ich keine bis sehr geringe Kenntnisse in HTML, CSS, Javascript und mit der Arbeit mit Express.js/node. Inzwischen würde ich unter Begutachtung meines Microservices sagen, dass meine Fähigkeiten in all diesen Gebieten mindestens gut geworden sind. Ich entschied mich bewusst, kein vorgefertigtes Responsive Design mit Bootstrap zu benutzen, weil ich es komplett selber machen wollte. Das Design so hinzukriegen, wie ich es wollte, hat sich als Herausforderung herausgestellt, die ich dennoch bewältigen konnte. Die wahre Herausforderung waren jedoch die Events und die generelle Arbeit mit JS am Server. Es hat viele Stunden gedauert, manche Funktionen fehlerfrei zum Laufen zu bekommen. Ich hatte zwar bereits damit gerechnet, doch praktisch war es dann noch mehr Zeit, die es benötigte. Aufgrund dessen habe ich dann nicht alle von mir geplanten Funktionen eingebaut bekommen.

Abseits der Software haben sich im Projekt meine Fähigkeiten in professioneller Arbeit im Team und Planung verbessern. Erkennbar ist dies vor allem dadurch, dass ich trotz ca. 1,5 Wochen Krankheit ein gut präsentierbares Ergebnis habe. Besonders half dabei, bei Problemen, bei denen ich allein nicht weiterkam, mich an Teamkollegen wie z. B. den Software-Architekten Andreas zu wenden.
Außerdem habe ich gelernt, dass eine gute Projektleitung einer der wichtigsten Aspekte eines Projekts ist. Unsere Produktivität steigerte sich dank der guten Arbeit der Projektleitenden mit der Zeit. Sie analysierten die Probleme jedes Sprints und versuchten diese im nächsten Sprint auszubessern.

- Fähigkeiten in JS/Express/CSS/HTML
- Professionalität ist wichtig für den Erfolg
- Abhängigkeiten voneinander erfordern gemeinsame Zeitplanung
- Software Projektmanagement war sehr hilfreich für dieses Modul
- Unterteilt in Microservices heißt absolut nicht, nicht gemeinsam arbeiten zu müssen

## Mattis Fieseler - Software Engineer
Am Anfang habe ich Payara als GlassFish Server verwendet, da wir in Webbasierte Application damit arbeiten
Ich habe auch einzelne Funktionen für die Queries zum Zugriff auf die Datenbank geschrieben wodurch sehr viel Code entstanden ist.

**Probleme mit CORS**<br>
Für Payara gibt es die Möglichkeit einen Header für jeden Request zu setzen, sodass Cross Origin Requests akzeptiert werden, allerdings hatte das bei mir nicht funktionieren wollen.
Nach mehreren Tagen habe ich mich dann dazu entschieden von Payara zu einem anderen Backend Server zu wechseln und mich für Spring entschieden, 
da ich mir hier von Clemens Hilfe holen konnte um mein Projekt initial umzubauen.<br>
-> Wechsel zu Spring<br>

Ich konnte schnell wechseln, da mit Plugins die bestehenden Datenbankmodelle erzeugt werden konnten und mit JPA wurde für die Abfragen von der Datenbank deutlich weniger Code benötigt.
Für Spring wurde das Backend in Service, Repository, Model und Controller aufgeteilt.
Außerdem kann durch die Anbindung zu Swagger die API Dokumentation übernommen werden.

Abseits von den technischen Schwierigkeiten habe ich gelernt, dass es sinnvoller wäre erst einen Bereich (z.B. Bibliothek) fertig zu stellen und dann die weiteren Module zu implementieren.

## Clemens Maas - Software Engineer

## Malte Kanders - Software Engineer

Als Software Engineer, als ein Full-Stack-Entwickler, am besten auch 
ohne jegliche Vorerfahrungen in irgendeinen dem erforderlichen Gebieten,
fühlt man sich ziemlich im Dunkeln. 
Gerade dann ist wohl meine wichtigste Lesson ein Modell der Entwicklung 
zu nehmen das bekannt ist und eine große Anzahl einer Community aufweist und
nicht ein Nischenprodukt, das eher aus den bekannteren aufgebaut ist.
Mein erster Ansatz mit dem Kotlin Projekt trug keine Früchte, eventuell
auch nur weil ich noch keine Ahnung mit der Webentwicklung hatte, oder 
auch, weil die Kotlin mäßige Webentwicklung noch nicht ausgereift genug ist.

Mit dem auf MERN Stack basierende System war es viel einfacher umzusetzen.
Man konnte sich genau Tutorials entlang hangeln und fand Hilfe bei 
größeren Software Portalen.

Eine weitere Sache unter den vielen Entwicklern.
Es ist schön, wenn jeder seine eigene Projektbasis hat und aufbaut.
Aber wahrscheinlich ist dieser Ansatz schlauer, wenn man nicht "Neuling" ist.
Es ist viel schwieriger zu helfen, wenn die Frameworks nicht viel von einander
haben und man selber ja genug zu tun hat.
