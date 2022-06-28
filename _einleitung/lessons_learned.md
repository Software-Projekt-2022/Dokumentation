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

## Andreas Wegner - Software Architekt, Software Engineer

## Jonas vom Braucke - Software Engineer

## Toni Schnittger - Software Engineer

## Mattis Fieseler - Software Engineer
Am Anfang habe ich Payara als GlassFish Server verwendet, da wir in Webbasierte Application damit arbeiten
Ich habe auch einzelne Funktionen für die Queries zum Zugriff auf die Datenbank geschrieben wodurch sehr viel Code entstanden ist.
**Probleme mit CORS**
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
Als einfacher Software Engineer unter vielen.


Als Software Engineer, als ein Full-Stack-Entwickler, am besten auch 
ohne jegliche Vorerfahrungen in irgendeinen dem erforderlichen Gebieten.
Fühlt man sich ziemlich im Dunkeln. 
Gerade dann ist wohl meine wichtigste Lesson ein Modell der Entwicklung 
zu nehmen das bekannt ist und eine große Anzahl einer Community aufweist und
nicht ein Nischenprodukt, das eher aus den bekannteren aufgebaut ist.
Mein erster Ansatz mit dem Kotlin Projekt trug keine Früchte, eventuell
auch nur weil ich noch keine Ahnung mit der Webentwicklung hatte, oder 
auch, weil die Kotlin mäßige Webentwicklung noch nicht ausgereift genug ist.

Mit dem auf MERN Stack basierende System war viel einfacher umzusetzen.
Man konnte sich an genau Tutorials entlang hangeln und fand Hilfe bei 
größeren Software Portalen.

Eine weitere Sache unter den vielen Entwicklern.
Es ist schön, wenn jeder seine eigene Projektbasis hat und aufbaut.
Aber wahrscheinlich ist dieser Ansatz schlauer, wenn man nicht "Neuling" ist.
Es ist viel schwieriger zu helfen, wenn die Frameworks nicht viel von einander
haben und man selber ja genug zu tun hat.
