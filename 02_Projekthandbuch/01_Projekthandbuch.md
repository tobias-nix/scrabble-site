# Projekthandbuch Scrabble  

## Historie
| Version | Status | Datum | Autor | Erläuterung |
| --- | --- | --- | --- | --- | 
| 0.1 | In Arbeit | 14.10.2023 | Nerb | Grundlagen des Projekthandbuchs eintragen | 


## Zusammenfassung

Das Projekthandbuch enthält alle notwendigen Informationen zum Projekt Scrabble und ist der Einstieg in das Projekt. Hier finden sich alle organisatorischen Informationen und Verweise auf notwengige Dokument. Außerdem wird das Projekt und der Projektkontext beschrieben.

## Einleitung

Zuerst wird der Zweck des Dokuments vorgestellt. Im Anschluss wird der redaktionelle Prozess erläutert und wer bei Änderungen informiert werden muss.

###	Zweck des Dokuments 

Das Projekthandbuch beschreibt das Projekt Scrabble und ist der Einstieg in die gesamte Dokumentation des Projekts. Es bietet einen Einleitung in das Projekt und informiert über die Rahmenbedingungen, die Projektorganisation sowie Planungen des Projektes. Das Dokument wird bei Bedarf im Projektverlauf aktualisiert. Zusätzlich sei darauf hingeweiesen, das das Projekthandbuch den Zughang zu sämtlichen für die Durchführung des Projekts relevanten Dokumente und Informationen beschreibt.


###	Redaktion
Verantwortlich für die Pflege des Projekthandbuchs ist der Projektleiter. Änderungen werden ausschließlich durch den Projektleiter eingebracht.   

###	Verteiler
Über Änderungen des Projekthandbuchs wird das gesamte Projektteam informiert. Dazu wird eine Mail an alle Projektbeteiligten (siehe Kapitel [Teamaufbau](#teamaufbau)) geschrieben.

## Projektdefinition

### Vorgeschichte 

Der Scrabble e. V. verfügt bisher nicht über die Möglichkeit, Scrabblespiele online auszutragen. Für diese Zwecke wurden stets Video- Gruppenchats verwendet, in denen ein Spieler das Brettspiel live übertrug. Zusätzlich mussten die Statistiken von den Gruppenmitgliedern manuell erfasst werden.

Ein erstes Kundengespräch hat am 11.10.2023 stattgefunden. Das Gesprächsprotokoll befindet sich im Ordner 01_Besprechungsprotokoll. 

###	Inhaltliche Kurzdarstellung

Die Anwendung Scrabble ist eine Server-Client-Applikation, die mithilfe von Java realisiert wird. Server und Client kommunizieren über RMI. Die Anwendung ermöglicht es Spieler:innen das Brettspiel Scrabble online, gemäß den allgemeinen Regeln zu spielen. Die Spieler:innen haben die Möglichkeit entweder eine Spielsitzung zu erstellen und diese für andere Mitspieler freizugeben.

###	Vertragsbasis

Das Projekt wird im Rahmen des Moduls „Secure Software Engineering“ erstellt. Es gelten die folgenden Rahmenbedingungen:

* Der wichtigste Bestandteil der Portfolio-Prüfung, da ein komplettes Software-Projekt im Team durchgeführt wird und Ihre Rolle im Team und die erstellten Produkte in die Bewertung einfließen.
* Aufteilung in Entwicklungsteams mit je 4-5 Teammitgliedern.
* Die Teams werden von Antje Neve und Andrea Baumann betreut. Der dem Team zugehörige Betreuer ist gleichzeitig der Kunde bzw. der Auftraggeber.
* Sie erhalten i.A. wöchentlich montags in der Vorlesung neue Aufgabenblätter, auf denen die vom Team zu erledigenden Aufgaben beschrieben sind. Diese Aufgabenblätter werden auch auf Ilias zur Verfügung gestellt.
* Pro Woche gibt es ein Treffen im Team mit Ihrer Betreuerin. Die Teams sollten sich nach Bedarf auch außerhalb dieses Termins treffen. 
* Jedes Team übernimmt eigenständig die Aufgabenplanung und Projektdokumentation. Planen Sie wer für welche Aufgaben zuständig ist und wer für welche Produkte zuständig ist. 
* Ihrer wöchentlichen Ergebnisse/Produkte werden beurteilt. Dazu gibt es zu den einzelnen Produkten Kontrollfragen, die wir zur Beurteilung und Sie zur Kontrolle Ihrer Ergebnisse verwenden.
* Alle erstellten Dokumente und Spurcecode müssen auf GitLab abgelegt werden: https://gitlab.dublin.etti.unibw.de 
* Ein komplettes Software-Projekt in so wenig Zeit durchzuführen ist eine große Herausforderung. Deswegen wird selbständiges Arbeiten und zeitnahe Kommunikationsbereitschaft bei auftretenden Problemen erwartet.
* Wieviele Punkte Sie für das Praktikum und die erstellen Produkte bekommen, hängt von den Teamtreffen, der Dokumentation und dem Sourcecode auf dem GitLab-Server ab.

Die Bewertung der Ergebnisse findet unter den folgenden Bedingungen statt:

* Insgesamt können Sie im Rahmen vom Praktikum und der anschließenden mündlichen Prüfung (30 Minuten) 225 Punkte erreichen.
* Im Praktikum selbst können Sie bis zu 150 Punkte sammeln und in der mündlichen Prüfung 75 Punkte. 
* Die Punkte im Praktikum setzten sich aus 100 Punkte, die Sie für Ihre Rolle und Ihre erstellten Produkte erhalten können, plus 50 Punkte, die Sie für zusätzliche projekttypische Aufgaben, erhalten, wie z.B. Review-Tätigkeiten, engagierte Teilnahmen an den Teamtreffen oder
Übernahme einer Doppelrolle.
* Ihre erreichten Punkte im Praktikum werden Ihnen vor der mündlichen Prüfung mitgeteilt.
* Mit dem Erreichen von 101 Punkten haben Sie die Portfolioprüfung mit 4,0 bestanden. Mit 191 Punkten haben Sie sich eine 1,0 verdient. 
* Fehlzeiten während des Praktikums müssen mir durch ärztliche Atteste oder einen Nachweis, dass das Fehlen nicht Ihre Schuld ist, belegt werden. Jedes unentschuldigte Fehlen reduziert die zu erreichende Punktzahl im Praktikum um 15 Punkte. Bitte denken Sie daran, dass Sie im Team arbeiten! 
* Fehlzeiten werden nach Absprache mit dem Team und der Betreuerin nachgearbeitet. 
* Sollten Sie die Prüfung nicht bestehen oder aus unverschuldeten Gründen nicht ablegen bzw. die Arbeit am Projekt nicht fertigstellen können, dann wird Ihnen im folgenden Trimester die Möglichkeit zur Wiederholung bzw. zur Nacharbeit gegeben.

###	Projektergebnis

Es müssen die folgenden Produkte erstellt werden: Projekthandbuch, Besprechungsprotokolle, Anforderungsspezifikation, Architekturdokument, Testspezifikation, Implementierung.

Für die Projektergebnisse sind die folgenden Abgabetermine vorgesehen:

| Vorlesung | Praktikum | Produkt | Abgabetermin |
| --- | --- | --- | --- | --- | 
| 09.10.2023 | 11.10.2023 | Besprechungsprotokoll, Projekthandbuch                  | 17.10.2023 (8Uhr) |
| 16.10.2023 | 18.10.2023 | Besprechungsprotokoll, Risikoliste                      | 24.10.2023 (8Uhr) |
| 23.10.2023 | 25.10.2023 | Besprechungsprotokoll, Anforderungsspezifikation        | 30.10.2023 (8Uhr) |
| 30.10.2023 | 31.10.2023 | Besprechungsprotokoll, Risikoliste                      | 07.11.2023 (8Uhr) |
| 06.11.2023 | 08.11.2023 | Besprechungsprotokoll, Architekturdokument              | 14.11.2023 (8Uhr) |
| 13.11.2023 | 15.11.2023 | Besprechungsprotokoll, Testspezifikation, Risikoliste   | 21.11.2023 (8Uhr) |
| 20.11.2023 | 22.11.2023 | Besprechungsprotokoll, JUnit-Tests                      | 28.11.2023 (8Uhr) |
| 27.11.2023 | 29.11.2023 | Besprechungsprotokoll, Implementierung                  | 05.11.2023 (8Uhr) |
| 04.12.2023 | 06.12.2023 | Besprechungsprotokoll, Testprotokoll, Touch-Down Folien | 12.11.2023 (8Uhr) |
| 11.12.2023 | 12.11.2023 | Alle                                                    |                   |

###	Informelle Ziele des Projektes

Die Projektbeteiligten sollen den Software Engineering Prozess und die wichtigsten Produkte der Softwareerstellung kennenlernen.

### Sonstige Besonderheiten

##	Risiken, besondere Rahmenbedingungen

Die Risiken und Maßnahmen finden sich in der Datei Risikoliste im Ordner 03_Risikoliste.

##	Projektorganisation

###	Teamaufbau

| Name | Rolle | Erreichbarkeit |
| --- | --- |  --- |
| Nerb              | Projektleiter             | simon.nerb@unibw.de          |
| Kompalka          | Anfoderungsanalyst        | jonas.kompalka@unibw.de      |
| Bößendörfer    | Fachliche Chefdesignerin  | anna.boessendoerfer@unibw.de |  
| Nix               | Testmanager               | tobias.nix@unibw.de          |
| Seegerer          | Systemarchitekt           | gabriel.seegerer@unibw.de    | 

Die Aufgaben der Teammitglieder entsprechend ihren Rollen sind wie folgt:

* **Anforderungsanalyst** und **fachlicher Chefdesigner**: Verantwortlich für das Anforderungsmanagement
    * Verantwortlich für die Anforderungsspezifikation: was soll das System leisten. • Wenn die Anforderungsspezifikation gut geschrieben ist, kann daraus mit relativ wenig Aufwand eine Benutzerdokumentation erstellt werden oder sogar direkt verwendet werden.
    * Der fachlicher Chefdesigner ist insbesondere für das fachliche Datenmodell verantwortlich.
    *  Anforderungsanalyst und fachlicher Chefdesigner in Personalunion bei weniger als 5 Teammitgliedern.
* **Systemarchitekt** und Entwicklungsteamleiter: Verantwortlich für die Systemarchitektur und die Umsetzung in Software
    * Verantwortlich für das Architekturdokument: Wie soll das System umgesetzt werden.
    * Verantwortlich für die Umsetzung bzw. die Implementierung entsprechend dieser Architektur.
    * Der Systemarchitekt ist insbesondere für das Komponentenmodell verantwortlich.
    * Entwicklungsteamleiter und Systemarchitekt in Personalunion bei weniger als 6 Teammitgliedern.
* **Testmanager**: Verantwortlich für die Testdurchführung
    * Verantwortlich für die Testspezifikation: Wie soll das System getestet werden.
    * Verantwortlich für die Erstellung der Testprotokolle.
* **Projektleiter**: Verantwortlich für den Projektablauf
    * Festsetzung der Projektstruktur und der Spielregeln im Projekthandbuch
    * Protokolliert den Kundenkontakt und plant den zeitlichen Ablauf und den Einsatz der Ressourcen und Teammitglieder. Die Ergebnisse werden in Besprechungsprotokollen festgehalten.
    * Protokolliert die Risiken des Projekts in der Risikoliste. Jedes Teammitglied ist natürlich nicht nur in seiner Rolle tätig, d.h. auch der Projektleiter kann als Software-Entwickler oder zum Testen eingeplant werden. „Verantwortlich" ist bitte nicht mit „arbeitet alleine" gleichzusetzten.

### Zusammenarbeit mit dem Kunden 

Der Projektleiter ist der Hauptansprechpartner für den Kunden. Alle Gespräche bzw. Absprachen mit dem Kunden müssen protokolliert werden. Die Protokolle müssen von beiden Seiten abgenommen werden.

Alle Mails und Dokumente müssen erst durch die Projektleitung frei gegeben werden, bevor diese an den Kunden verschickt werden.

Auf der Kundenseite steht und Frau Prof. Baumann (andrea.baumann@unibw.de) zur Verfügung.

### Besprechungen

Es finden wöchentliche Treffen mit dem Kunden/der Kundin statt. An diesem Treffen nehmen alle Teammitglieder teil. Die Treffen sind immer am Mittwoch um 08:00 Uhr in Raum 33/1414. In diesem Rahmen werden wöchentlich auch alle Projektrisiken besprochen. Die Ergebnisse müssen immer in einem Besprechungsprotokoll festgehalten werden.

Unsere internen Besprechungen finden jeweils nach diesen Treffen statt. Die Ergebnisse werden in einem internen Besprechungsprotokoll festgehalten. Bei den internen Besprechungen werden auch die Risiken besprochen, die nicht für die Ohren des Kunden bestimmt sind.
Besteht kein Bedarf für ein Kundentreffen, dann muss dies mit dem Kunden abgesprochen werden und die Teilnehmer:innen rechtzeitig darüber informiert werden.

## Planungen

### Projektplan und Meilensteine

| Termin | Schwerpunkt |
| --- | --- | --- | 
| 11.10.2023 | Kickoff und erste Anforderungen                  |
| 18.10.2023 | Anforderungen sammeln/aufschreiben               |
| 25.10.2023 | Anforderungsspezifikationen fertigstellen        |
| 31.10.2023 | Architektur planen/aufschreiben                  |
| 08.11.2023 | Architekturdokument fertigstellen                |
| 15.11.2023 | Test planen/Testdokument erstellen/fertigstellen |
| 22.11.2023 | JUnit-Test erstellen/Implementierung beginnen    |
| 29.11.2023 | Implementierung fertigstellen                    |
| 06.12.2023 | Integration und Abnahme/Touch-down vorbereiten   |
| 12.12.2023 | Touch-down: Projekt abschließen                  |

### Restaufwandschätzung

## Qualitätssicherung

## Datenschutz

In unserem Projekt gibt es keine besonderen Datenschutzrichtlinien die beachtet werden müssen.

## Dokumentation und Ablage

Im gesamten Projektverlauf ist auf eine saubere und konsistente Ablage aller erstellten Produkte und relevanten Dokumente zu achten.
Alle Daten werden in einem Versionsverwaltungssystem gespeichert. Dabei gibt es zwei zentrale Projekte.

**Dokumentation** über GitLab auf ein zentrales Git-Repository: 
  https://gitlab.dublin.etti.unibw-muenchen.de/edu-sse-2023-team-d/scrabble-site.git    
  Hier wird die gesamte Dokumentation gespeichert, die mit Markdown und Excel erstellt wurden.

**Sourcecode** über GitLab auf ein zentrales Git-Repository: : 
https://gitlab.dublin.etti.unibw-muenchen.de/edu-sse-2023-team-d/scrabble-src.git   
Hier wird der entwickelte Sourcecode gespeichert. Sowohl die Client- als auch die Sever-Enwicklung.

Zur **Dokumentation** des Projekts mit Markdown:
https://code.visualstudio.com

Zur **Programmierung** des Projektes  mit Java:  https://www.jetbrains.com/idea/

Zur **Kommunikation mit dem Kunden**:
https://mattermost.dublin.etti.unibw-muenchen.de/edu-se/channels/secure-software-engineering

Zur **teaminternen Kommunikation**:
https://discord.com/invite/R2KxFX3U 
https://mattermost.com 

Zur Bearbeitung von **UML Diagramm**:
https://www.visual-paradigm.com

Designentwurf der **Oberflächen**:  https://www.drawio.com       

## Referenzliste

* Allgemeinen Spielregeln: https://scrabble-info.de/wp-content/uploads/2016/03/Allgemeine-Scrabble-Spielregeln.pdf
* Spielbrett: https://de.wikipedia.org/wiki/Scrabble#/media/Datei:Scrabbleboard.svg
* Spielsteine: https://en.wikipedia.org/wiki/Scrabble_letter_distributions




## Abkürzungsverzeichnis und Glossar

