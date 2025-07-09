---
title: Support Prozesse
description: Hier werden alle Prozesse für den Support erläutert damit jeder weiß was zu tun ist
published: true
date: 2025-07-09T09:54:25.366Z
tags: 
editor: markdown
dateCreated: 2025-07-09T09:54:14.171Z
---

\# i-doit support process

\## Support roles

\### First Level Support

\*\*Telefonischer Support\*\*<br>

Ansprechpartner für telefonische Anfragen. Vertreten durch die anderen. Kümmert sich um die Slack Telefonzentrale, wenn @care-team dort markiert wird oder nach ~15:30 Uhr.

\*\*Schnittstelle zur Entwicklung "3rd Level Meeting"\*\*<br>

Das 3rd Level Meeting findet täglich zusammen mit einem Kollegen aus der Entwicklung statt. Der 1st-Level-Supporter übernimmt die Abstimmung aller Care relevanten Themen mit der Entwicklung. Alle der Entwicklung (3rd level) zugewiesenen Tickets werden im Jour Fix besprochen und bekommen eine Status Update. Absprachen, Leistungszeiträume oder andere relevanten Informationen werden als interne Notiz dem Ticket hinzugefügt. Im Anschluss an das Meeting werden die relevanten Informationen an die Kunden oder Kollegen weitergegeben.

Vor der Abgabe der Rolle des 1st-Level-Supporters erfolgt eine direkt Übergabe der relevanten Vorgänge an den Nachfolger.

Der First Level Support ist so lange er die Funktion ausführt der primäre Ansprechpartner auf den jeweiligen genutzten Kommunikationswegen. Die Rolle des First Level Supporters wechselt innerhalb des Teams wöchentlich und ist in den jeweiligen Kalendern ersichtlich

\---

\### Second Level Support

Der Second Level Support richtet sich in der Regel an die Leitung des Care Teams oder andere Kollegen die nicht Mitglied des Care Teams sind. Hier geht es um Fachfragen zu unseren eigenen Add-ons, Produktentscheidungen oder auch eskalationen die das Eingreifen der Team Leitung erfordern.

Der Second Level Support bekommt seine Tickets aus dem First Level Support übergeben. Die Tickets sind in der Regel vorqualifiziert und beinhalten alle Informationen um mit einer zügigen bearbeitung zu beginnen. Fehlern hier auf den ersten Blick schon Informationen werden die Tickets zur Revision in den First Level zurück geroutet.

\---

\### Third Level Support

Der Third Level wird durch die Entwicklungsabteilung abgedeckt. Hier geht es primär um Fragen die Einsicht und Verständnis in den Code erfordern, wie z.B. das beheben von Bugs oder die Erklärung von Parametern und Funktionen.

\---

\### Sprint Partner

Die Entwicklung plant die Aufgaben in kleine zeitliche Abschnitte. Diese werden Sprints genannt und laufen in der Regel über einen Zeitraum von zwei Wochen. Die Priorisierung der Themen, die im jeweils nächsten Sprint erledigt werden wird von Care vorgenommen. Hierbei sollen Dringlichkeiten berücksichtigt und dafür gesorgt werden, dass die Priorisierung der offenen Themen sinnvoll vorgegeben wird.

Die verfügbaren Ressourcen aus dem Entwickler-Team werden auf Basis der offenen Bugs festgelegt. Care ist dafür verantwortlich, diese Zahlen aufzubereiten, in einer Übersicht festzuhalten und vor der Sprintplanung zu präsentieren. Weiterhin werden, abhängig von diesen Statistiken die Story Points in entsprechender Menge auf den Sprint verteilt.

Während des Sprint-Meetings werden diese im Product-Team präsentiert, gemeinsam geprüft und freigegeben.

\---

\## Kommunikationswege

Die folgenden Kommunikationswege stehen zur Verfügung und werden genutzt

\_\*\*Primär\*\*\_

\*\*E-Mail\*\*

\*\*Ticketsystem\*\*

\*\*Telefon\*\*

\*\*Slack\*\*

\---

\## Ticketannahme und Kontrolle

\### Definitionen

Neue, eingehende Tickets sind auf vollständigkeit zu überprüfen und zu Kategorisieren. Hier gilt als Maßstab die innerhalb des Care Teams festgelegten Felder mit den Mindestinformationen zu füllen:

| Information Kurzname | Beschreibung                                          | wird geliefert von             |

| -------------------- | ----------------------------------------------------- | ------------------------------ |

| Anfragender          | vollständiger Name, email Adresse                     | Salesforce/Kunden              |

| Firma                | Firmenname                                            | Salesforce/Zendesk mail domain |

| Mitarbeiter          | Der aktuell zuständige Mitarbeiter                    | Care                           |

| CCs                  | Mitleser für Ticketverlauf                            | optional bei Bedarf            |

| Priorität            | Priorität, errechnet aus Dringlichkeit und Auswirkung | Zendesk                        |

| Stichworte           | sinnvolles Tagging                                    | Care                           |

| Typ                  | Art der Anfrage                                       | Care                           |

| Supportoption        | Supportvertrag Ohne, Basic, Advanced                  | Salesforce                     |

| Version              | i-doit pro Verison                                        | Kunde/Care                     |

| Server OS            | Server Betriebssystem des Kunden                      | Kunde/Care                     |

| Browser              | Browser Version des Kunden                            | Kunde/Care                     |

| Dringlichkeit        |                                                       |                                |

| Auswirkung           |                                                       |                                |

| Eskalationsstufe     | Kategorisierung der Eskalationsstufe                  | Care                           |

| 3rd Level Info       | Information zum 3rd Level Zustand                     | Care/Entwicklung               |

|                      |

Sollten hier absehbar für die Beantwortung wichtige Informationen fehlen sind diese durch den 1st-Level-Supporter beim Anfragenden durch rückfrage anzufordern.

Für die Nachstellung von unerwünschtem Verhalten innerhalb von i-doit pro sind die für die Nachstellung des Problems verwendeten Materialien mitzuliefern. ( z.B. CSV Datei bei einem Import Fehler)

Bei Fehlern in der Benutzeroberfläche sind entsprechende Screenshots des Fehlverhaltens mitzuliefern.

Wenn es sich bei der Anfrage um eine Wissensfrage handelt die ohne weiteres schnell beantwortet werden kann, z.B. durch das zusenden eines Links auf die Knowledge Base, ist diese direkt zu beantworten. Komplexere Anfragen werden an den Second Level weitergeleitet.

Nach Prüfung aller genannten Kriterien ist das Ticket, soweit es nicht direkt beantwortet werden kann, an den Second Level Support weiterzuleiten. Bei eskalativen Themen ist der Second-Level-Support direkt zu informieren und zu alarmieren.

\---

\### Automatisierte Ticketpriorisierung

Tickets werden anhand der Attribute Dringlichkeit, Auswirkung und Ruhezeit priorisiert.<br>

Die Priorisierung erfolgt initial und automatisiert, sobald die Werte Dringlichkeit und Auswirkung bekannt sind.

Die Priorisierung nach Ruhezeit erfolgt durch eine spätere zeitliche Eskalation und wird in den Lösungsprozessen beschrieben.

Die initiale Priorisierung und deren Auswirkung erfolgt nach folgender Matrix:<br>

(sofern auch mit Documentum entsprechende Support Level existieren werden)

|               |     | Auswirkung | Auswirkung | Auswirkung |

| ------------- | --- | :--------: | :--------: | :--------: |

|               |     |     H      |     M      |     N      |

| Dringlichkeit | H   |     1      |     2      |     3      |

| Dringlichkeit | M   |     2      |     3      |     4      |

| Dringlichkeit | N   |     3      |     4      |     4      |

| Priorität | Beschreibung | Reaktionszeit-Vorgabe | Lösungszeit-Vorgabe |

| :-------: | :----------: | :-------------------: | :-----------------: |

|     1     |   Dringend   |        Sofort         |      8 Stunden      |

|     2     |     Hoch     |       4 Stunden       |     16 Stunden      |

|     3     |    Normal    |       8 Stunden       |     24 Stunden      |

|     4     |   Niedrig    |      24 Stunden       |     40 Stunden      |

Die Reaktionszeiten gelten jeweils während der Arbeitszeit, d.h. 24 Stunden Reaktionszeit entspricht drei Werktagen. Die Reaktions- und Lösungszeiten sind von uns intern gelebte, nicht veröffentlichte Werte.

\---

\### Einfluss des Supportvertrages

Bei Eingang eines Tickets wurde bisher automatisiert festgestellt, ob der Anwender einen gültigen Supportvertrag besitzt. Wenn ja, wurde dieses im Ticket vermerkt und die Dringlichkeit gesetzt.<br>

Dabei galt:

\- Hat der Anwender Advanced Support, wird die Dringlichkeit auf "Hoch" gesetzt.<br>

\- Hat der Anwender Basic Support, wird die Dringlichkeit auf Mittel gesetzt, sofern er sie nicht manuell auf "Hoch" gesetzt hat.<br>

\- Ist der Anwender als Evaluierend geflagged, wird die Dringlichkeit auf "Hoch" gesetzt.

\---

\### Initiale Priorität bei Eingang

Die Priorität eingehender Tickets wird anhand ihrer Dringlichkeit gesetzt, solange keine Auswirkung definiert wurde.

\---

\### Zeitliche Eskalation von nicht bearbeiteten Tickets

Alle Tickets werden stündlich auf Aktion abgefragt und ggf. bei Nichtreagieren eskaliert.<br>

Dabei gilt folgende Matrix für die Zeit:

\- vom Eingang eines Tickets bis ein Mitarbeiter zugeordnet wird<br>

\- vom Zuweisen eines Mitarbeiter bis zur Lösung

| Unangetastet oder Offen seit |  Priorität   |  Priorität   | Priorität | Priorität |

| :--------------------------: | :----------: | :----------: | :-------: | :-------: |

|          0 Stunden           | \*\*Dringend\*\* |    \_Hoch\_    |  Normal   |  Niedrig  |

|          8 Stunden           | \*\*Dringend\*\* | \*\*Dringend\*\* |  \_Hoch\_   |  Normal   |

\*\*Daraus ergeben sich folgende Regeln:\*\*

| Unangetastet/Offen seit | initiale Priorität | neue Priorität |

| :---------------------: | :----------------: | :------------: |

|           8H            |     \_NIEDRIG\_      |   \*\*NORMAL\*\*   |

|           16H           |     \_NIEDRIG\_      |    \*\*HOCH\*\*    |

|           24h           |     \_NIEDRIG\_      |  \*\*DRINGEND\*\*  |

|           8H            |      \_NORMAL\_      |    \*\*HOCH\*\*    |

|           16H           |      \_NORMAL\_      |  \*\*DRINGEND\*\*  |

|           24h           |       \_HOCH\_       |  \*\*DRINGEND\*\*  |

Für den Advanced Support gibt es eine gesonderte Regel, da wir hier zu einer Reaktionszeit von 4h verpflichtet sind.<br>

Alle Zeiten werden auf Basis der Geschäftszeiten gerechnet.<br>

\_Die Berechnung endet dann,\_

\- wenn in einem Ticket ein Mitarbeiter zugeordnet wird und das Ticket von "Neu" auf den Status "Offen" gesetzt wird. In diesem Moment wird auch die Priorisierung wieder auf die normale Berechnungsgrundlage zurückgesetzt.<br>

\- wenn der Mitarbeiter das Ticket auf Gelöst setzt

\---

\### Mitarbeiterzuweisung

Mit der Zuweisung eines Tickets und einstellen mit dem Status "Offen" startet die Bearbeitung eines Tickets. Der Anfragende wird über diesen Schritt informiert (Informationsmail: Ticket ist in Bearbeitung)

\---

\## Ticket Kategorisierung

\### Kategorisierung Inhaltliches Problem

Der erste Schritt in der Bearbeitung eines Tickets ist die Kategorisierung nach inhaltlichem Problem (Verständnisfrage) oder nach technischem Problem.<br>

Inhaltliche Probleme sind meistens einfach zu identifizieren.<br>

Im Ticket muss dann entsprechend das Feld "Typ" auf "Inhaltliches Problem" gesetzt werden.<br>

Die Bearbeitung nach der Prozessvorgabe "Lösung Inhaltliches Problem" wird zur Lösung des Problems gestartet.

\### Kategorisierung Bug Report

Ist das Problem reproduzierbar, handelt es sich um einen Bug Report.<br>

Im Ticket muss dann entsprechend das Feld "Typ" auf "Bug Report" gesetzt werden.

Die Bearbeitung nach der Prozessvorgabe "\[Lösung Bug Report\](#lösung-bug-report)" wird zur Lösung des Problems gestartet.

\### Kategorisierung Individuelles technisches Problem

Lässt sich das Problem auf einer Standardumgebung nicht reproduzieren, handelt es sich um ein individuelles technisches Problem.<br>

Im Ticket muss dann entsprechend das Feld "Typ" auf "Individuelles technisches Problem" gesetzt werden.<br>

Die Bearbeitung nach der Prozessvorgabe "Lösung Individuelles technisches Problem" wird zur Lösung des Problems gestartet.

\### Feature Feedback (früher Feature Request)

Ist ein eintreffendes Ticket auf den ersten Blick schon als Feature Request zu kategorisieren wird dieses direkt durch den 1st-Level-Supporter erledigt, beantwortet und in Jira eingetragen. Der Kunde bekommt eine Antwortmail in der wir uns für das wertvolle Feedback bedanken und das wir, sollten wir uns dem Feature widmen, die Kommunikation wieder aufnehmen.

Die Bearbeitung nach der Prozessvorgabe "Lösung Feature Feedback" wird zur Lösung des Problems gestartet.

\### Kategorisierung Partner Add-On

Liegt ein Problem an einer Schnittstelle oder einem Add-On eines Partners, wird zum Partner eskaliert. Hier sind aktuell noch keine Add-ons von Partnern bekannt, sobald hier Add-Ons verfügbar sind muss dieser Prozess noch einmal in abstimmung mit dem Partner hinterfragt werden.

Wir leiten Anfragen dazu an die Partner weiter.

\### Kategorisierung Nicht zuständig

Ist der Support für das Problem nicht zuständig, wird der Status auf "Nicht zuständig" gesetzt.

\### Tickets ISMS & VIVA Becon

Link zum Dokument <https://docs.google.com/document/d/1BDbH5ZC93yBLf5liigAoYb3rhII6MDi9vOT1AURsnzo>.<br>

Tickets werden im Zendesk entgegengenommen.<br>

Es wird das Makro "BECON ISMS Übergabe" ausgeführt welches:

Eine Antwort an den Kunden schickt und ihn darüber informiert:

\`\`\`txt

"Sehr geehrter i-doit pro Kunde,

Ihre Anfrage bezieht sich auf ein Add-On welches nun von unserem Partner, der Becon GmbH aktuell weiterentwickelt wird, daher haben wir Ihr Anliegen an die Kollegen übermittelt.

Den Blogeintrag dazu finden Sie hier:

<https://www.i-doit.com/blog/premium-partner-becon-gmbh-uebernimmt-isms-und-viva2-add-on-von-synetics/>

Ihr Anliegen wird von der Becon GmbH begutachtet und Sie erhalten innerhalb dieses Tickets zeitnah eine Antwort mit allen weiteren Informationen.

Sollten Sie in der Zwischenzeit weitere Erkenntnisse nachreichen wollen antworten Sie einfach auf diese Nachricht oder innerhalb des Help centers unter:

https://help.i-doit.com

Mit freundlichen Grüßen

Kind regards"

\`\`\`

Das Ticket an den Support der Becon unter:  \`i-doit.support@becon.de\` weitergeleitet<br>

Weiterhin wurde der manuelle Prozess mit Becon / Jakob Semere getroffen:

\- es erfolgt eine Bestätigung im Becon \[ext-becon Slack Channel\](https://app.slack.com/client/T5XB3R6LF/CL31WD2P5) über den Erhalt des Zendesktickets im Ticket System der Becon

\- es erfolgen Meldungen über die Entwicklung des Tickets im Slack Channel

\- es wird der Abschluss des Support Falls im Slack Channel bekanntgegeben

Das Care Team überwacht die offenen "Becon Tickets" und erfragt bei ausbleiben von Aktualisierungen den aktuellen Stand.

\### Tickets Checkmk 2 Add-on SHD

Tickets werden im Zendesk entgegengenommen und bearbeitet. Sollte sich heraustellen, dass das Problem im CMK2 Add-on entsteht wird es an die SHD weitergeleitet.<br>

Es wird das Makro \`SHD CheckMK Übergabe\` ausgeführt welches eine Antwort an den Kunden schickt und ihn darüber informiert.<br>

Zusätzlich soll im CC \`synetics.support@shd-online.de\` und \`robert.friessleben@shd-online.de\` eingetragen werden.

Die Kollegen wünschen sich, dass wir wenn ein CMK2 Ticket gelöst wurde wir die Themen und die Lösung im \[ext-shd Slack Channel\](https://i-doit.slack.com/archives/C03S2AENZLP) posten.

Die Doku soll aktuell noch bei uns gehostet werden. Außerdem wird diese im CMK2 Paket enthalten und aktualisert werden.

\## Ticket Lösung

\### Lösung Inhaltliches Problem

Inhaltliche Probleme werden individuell vom Support-MA bearbeitet. D.h. mithilfe von KB Einträgen, Nachstellen, nachfragen wird eine Lösung gefunden.<br>

Die Lösung wird dem Anwender mitgeteilt und falls notwendig auf positives Feedback gewartet. Dazu wird das Ticket in den Status Wartend gesetzt.<br>

Nach Antwort wird das Ticket manuell auf "gelöst" gesetzt und der Anwender informiert<br>

Lösung zu inhaltliche Problemen werden, wenn sinnvoll, zu FAQ Artikeln verarbeitet oder in der KB hinterlegt.

\### Lösung Bug Report

Bug Reports werden jeweils auf einer eigenen Cloud Instanz die der Umgebung des Kunden entspricht nachgestellt.

Der nachgestellte Bug wird als Ticket in JIRA angelegt und mit Screenshots dokumentiert sowie textlich eindeutig beschrieben. Die Informationen müssen ausreichen, dass jemand Drittes den Fehler nachvollziehen kann, ohne weitere Nachfragen stellen zu müssen.

\_Folgende Attribute werden in JIRA zu einem Bug Report verpflichtend geliefert:\_

\- Priorität (dabei gilt: ZenDesk Ticketpriorität ist zu übertragen)

\- Beschreibung Deutsch

\- Beschreibung Englisch

\- i-doit pro Version

\- Beschreibung

\- Screenshots

\- Link zu Installation/Mandant

\- Ggf. weitere Anhänge

Das neue in JIRA erstellte Ticket wird mit dem ZenDesk Ticket verknüpft. Ist der Bug bereits bekannt, wird das bereits erstellte Jira Ticket verknüpft.<br>

Der Anwender wird hiervon automatisiert in Kenntnis gesetzt<br>

Das Ticket wird in den Status Wartend und auf die Eskalationsstufe "Developement/Entwicklung"gesetzt.<br>

Ab diesem Zeitpunkt wird das Ticket in der Entwicklung bearbeitet.<br>

Erfolgt in JIRA eine Lösung, wird automatisch das ZenDesk Ticket auf gelöst gesetzt. Der Anwender bekommt eine Information über die Version, mit der die Lösung veröffentlicht wird

\### Lösung individuelles technisches Problem

Bei individuellen technischen Problemen versucht der Support MA durch eigene Recherche eine Lösung zu finden.<br>

Dazu kann es nötig sein, die Umgebung des Anwenders mit oder ohne die Datenbank nachzustellen. Die Übertragung der Anwenderdaten erfolgt in individueller Absprache und Genehmigung des Anwenders.<br>

Ggf. wird eine \[Teamviewer\](https://get.teamviewer.com/i-doit) Remotesupport Session mit dem Anwender vereinbart, um das Problem zu lösen.<br>

Kann der MA eigenständig keine Lösung finden, eskaliert er das Ticket zum 2nd Level. Siehe Eskalation 2nd Level.<br>

Findet der 2nd Level ebenfalls keine Lösung, eskaliert er zum 3rd Level.

\### Siehe Eskalation 3rd Level

Die Lösung wird dem Anwender mitgeteilt und falls notwendig positives Feedback gewartet, dazu wird ggf.das Ticket in den Status Wartend gesetzt.<br>

Das Ticket wird auf "Gelöst" gesetzt, der Anwender informiert

\### Lösung Feature Feedback

Feature Requests werden in JIRA als Ticket angelegt und mit dem ZenDesk Ticket verknüpft.

Die Beschreibung des JIRA Tickets soll eindeutig nachvollziehbar sein.<br>

Der Anwender wird über die Aufnahme des Feature Requests automatisch informiert<br>

Das ZenDesk Ticket wird direkt auf gelöst gesetzt.<br>

Wird das JIRA Ticket gelöst, wird der Anwender über die Version, in der die Implementierung erfolgt, automatisch informiert.

\### Lösung Partner Add-On

Partner Add-on Tickets werden zum Partner eskaliert und wir kommunizieren die Antworten in Richtung des Kunden.

\### Lösung nicht zuständig

Die zuständige Abteilung wird über Slack über den Ticket Eingang benachrichtigt und gibt das weitere vorgehen über ein Kommentar des Slack Postings vor. Folgendes vorgehen ist hier vorgesehen:

\- Es bestehen noch Rückfragen seitens der Abteilung, das Care Team holt über das Ticket weitere Informationen ein.

\- Kommunikation wird von der jeweiligen Abteilung übernommen, wir geben dem Kunden bescheid das das Ticket übergeben wurde und schließen das Ticket.

\---

\## Automatismen und Eskalationen

\### Grundsätzlicher Ablauf im Ticketsystem

\- Tickets werden vom Anwender im Status \*\*"Neu"\*\* eröffnet

\- Nach Zuweisung eines Mitarbeiters und Start der Bearbeitung gelangt das Ticket in den Status \*\*"Offen"\*\*

\- Ist eine Eingabe eines Anwenders notwendig, geht das Ticket in den Status \*\*"Wartend"\*\*

\- Löst der Support MA das Ticket, stellt er es auf den Status \*\*"Gelöst"\*\*

\- Nach einer Wartezeit im Status "Gelöst" oder "Wartend" wird es automatisch auf \*\*"Geschlossen"\*\* gesetzt

\### Automatisiertes Schließen eines Tickets bei Nichtreaktion

Ist ein Ticket im Zustand Wartend und nicht vom Typ "Bug Report", wird nach 7 Tage (Kalenderzeit) ein E-Mail Reminder an den Anwender geschickt, dass das Ticket auf Eingabe wartet und ggf. automatisch geschlossen wird.<br>

Reagiert der Anwender weitere 7 Tage (Arbeitszeit) nicht, wird das Ticket automatisch auf "Geschlossen" gesetzt und der Anwender per E-Mail informiert

Automatisiertes Schließen eines Tickets nach Lösung<br>

Ist ein Ticket auf gelöst gesetzt, wird es nach 14 Tage (Kalenderzeit) automatisch geschlossen.<br>

Feature Requests sind hiervon ausgenommen, diese bleiben 365 Tage lang auf dem Status gelöst, bis sie geschlossen werden.<br>

Der Anwender wird hierüber nicht informiert.

\### Eskalation zum 2nd Level

Der 2nd Level ist derzeit nicht personell und inhaltlich definiert und wird vom 1st Level wahrgenommen. Trotzdem setzen wir jetzt schon eine Abgrenzung ein, um uns hier in Zukunft zu verbessern.<br>

Wird ein Ticket in den 2nd Level eskaliert, muss das Feld Eskalationsstufe auf "2nd Level" gesetzt werden.

\_Abgrenzung zum 1st Level:\_

\- 1st Level kann das Problem nicht lösen (unzureichende Kompetenz)

\- Das Ticket ist zeitaufwändig in der Nachstellung

\- Das Ticket ist zeitaufwändig oder eskaliert in der Kommunikation oder im Inhalt

\### Eskalation zum 3rd Level

Sobald ein Ticket von Care nicht eigenständig gelöst werden kann und Kompetenz aus dem DEV-Team gefragt ist wird dieses in den 3rd Level verschoben.

\### Eskalations Prozess Dev-Team

1\. Kunde erstellt Zendesk Ticket, dieses wird im Falle eines Fehlers durch Care entsprechend der Klassifizierungen (Seite 2) übertragen.

2\. Sichtung morgens aller am Tag vorher erstellten Tickets (bis 17:00) und Bewertung dieser bzgl. Priorität, Abhängigkeiten und Machbarkeit im Rahmen der Klassifizierungen (z.B. benötigt Feature), sollten Tickets in bestimmten Klassifizierungen erstellt werden welche eine frühere Reaktion benötigen, so gibt es für diese Klassifizierungen Filter die per Email benachrichtigen (Business Blocker z.B. alle 15min)

3\. Kunde wird anhand der Bewertung von Entwicklung durch Care transparent und verbindlich informiert. Entweder im Rahmen der Klassifizierungen oder in Form einer Ausnahme, z.B. Bug benötigt Feature welches geplant ist für Q3, Lösungszeit also 3 Monate bis Major Release, an den Kunden wird lediglich die verbindliche Lösungszeit kommuniziert.

4\. Sollte wider Erwarten im Rahmen der Klassifizierungen ein zuvor kommunizierter Leistungszeitraum nicht einhaltbar werden, so wird der Kunde frühzeitig vor Ablauf des Lösungs Zeitraumes informiert, dies soll die bisherigen Beschwerden verhindern.

  \*\*Altlasten:\*\*

  Beschwert Kunde sich über erneute "Nicht Lösung" oder zu langes warten seines Tickets wird von Care persönlich zur Entwicklung eskaliert (z.B. Slack, P2P), vorzugsweise im dev-consult in Slack.

5\. Erstellte Hotfixes werden nur im JIRA-Ticket hinterlegt.

  Format: JIRA-ID\_COMMIT-ID.zip

  Beispiel: ID-1234\_913ef2.zip

\### Sonderfälle

\- Critical/Major kurz vor Code-Freeze - kommt nicht in das kommende Release, aber in das nächste Release. Ticket wird auf Blocker hochgestuft und Hotfix wird für den Kunden vorbereitet.

\- Wird die Priorisierung aufgrund des Kunden angepasst, soll dies mit einem Kommentar im Ticket vermerkt werden. (z.B. laut Beschreibung Major, Kunde möchte aber zwingend einen Patch, dann wird dies zu einem Blocker)

\- Care versieht Bugs welche innerhalb des Code-Freezes identifiziert werden mit dem Label \`FeatureFreezeBug\` zur klaren Abgrenzung.

\### Klassifizierungen

In der Anfangsphase wird es keine definierten Lösungszeiten und auch keinen verpflichtenden Hotfix geben, die Lösungszeit und die Entscheidung "Pro Hotfix" wird von Produkt/DEV/Tech-Ops vorgegeben.

| Name | Eskalationsstufe                                                            | Typ              | Beschreibung                                                                                                                                                                                                             | Lösungszeit      | Hotfix? |

| ---- | --------------------------------------------------------------------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------- | ------- |

| FK1  | unmittelbare Info an GF, Produkt- management und Supportleitung             | Business Blocker | die zweckmäßige bzw. wirtschaftlich sinnvolle Nutzung der Software gemäß Dokumentation ist nicht möglich oder so eingeschränkt, dass die Abwicklung des Tagesgeschäfts des Kunden nicht zumutbar fortgeführt werden kann |                  |         |

| FK2  | einmal tägliche Zusammen- fassung an Produkt- management und Supportleitung | Blocker          | die zweckmäßige bzw. wirtschaftlich sinnvolle Nutzung der Software gemäß Dokumentation ist erheblich eingeschränkt, die Abwicklung des Tagesgeschäfts des Kunden ist jedoch noch möglich                                 |                  |         |

| FK3  |                                                                             | Critical         | die zweckmäßige bzw. wirtschaftlich sinnvolle Nutzung der Software gemäß Dokumentation ist nur unwesentlich, d.h. ohne nennenswerte Auswirkungen auf die Funktionalität des Gesamtsystems                                |                  |         |

| FK4  |                                                                             | Major            | sonstige Fehler, d.h. Unvollkommenheiten der Software, die deren Funktionalität nicht beeinträchtigen, die jedoch störend in Erscheinung treten                                                                          | nächstes Release |         |

| FK5  |                                                                             | Minor            |                                                                                                                                                                                                                          |                  | -       |

\### Erstellung von Hotfixes

Wird für ein Ticket ein Hotfix benötigt, dann wird dazu ,im erstelltem Jira Ticket, das Feld \`Hotfix notwendig?\` auf \`Ja\` gestellt.<br>

Außerdem wird das Ticket in die Jira queue aka \[Backlog\](https://i-doit.atlassian.net/jira/software/c/projects/ID/boards/41/backlog?issueLimit=100#:~:text=%F0%9F%9A%A8-,Emergency%20Tickets,-%F0%9F%9A%A8) "🚨 Emergency Tickets 🚨" gesetzt.<br>

Anschließend informieren wir den i-doit PO (Jens Dörnenburg) und die Devs im \[dev-Consult Slack Channel\](https://join.slack.com/share/enQtNTQzMzY1NTEyOTcxOS0zNDM0NmViNGNlMDA3NjZkYzc2ZjNlY2EzNDhjZDQzZjkxZWU1Yzg3MTcyYWQyYTRhOWRhNWI0N2VkMWY3MmM3) indem wir Sie mention via @.

Wurde ein Hotfix erstellt, wird dieser jedem Kunden zugeschickt, der am Jira Ticket verknüpft ist.<br>

Außerdem wird der Hotfix der Knowledge Base hinzugefügt. Dies geschieht z.B. im Bereich \`Deutsch\` unter \[Hotfixes\](https://kb.i-doit.com/de/administration/hotfixes/index.html).<br>

\### Datenaustausch mit Anwendern

Der Datenaustausch mit Anwendern geschieht über ZenDesk Ticket Attachments im Portal (SSL gesichert) bzw. über E-Mail Anhänge. Bei größeren Datenmengen müssen individuelle Übertragungen vereinbart werden.

\### JDisc daten nicht vorhanden (keine Reproduktion möglich)

Fehlen Daten, um das Problem des Kunden reproduzieren zu können, in unserer JDisc Datenbank, dann wird das \*\*REQ - Bitte um JDisc Daten\*\* Makro verwendet.

Dies zeigt dem Kunden einen Weg auf z.B. einzelne Objekte zu exportieren.

Sind die Daten vorhanden werden Sie auf dem \[JDisc Host für den Support\](https://doku.synetics.int/?viewMode=1001&objTypeID=138) eingespielt. Wurde der Bug gelöst sind die Daten zu löschen.

\### Anwender Feedback einholen

Anwender Feedback wird 24 Stunden nach Schließen eines Tickets vom Benutzer angefordert. Es gibt nur zwei Bewertungskriterien: Gut oder schlecht. Jede Art der Bewertung kann mit und ohne Kommentar (Freitext) abgegeben werden. Bei einer negativen Bewertung steht außerdem eine Auswahl von Standard-Gründen per Drop-Down zur Verfügung, die alternativ zum Freitext ausgewählt und so genutzt werden kann.<br>

Die Auswertung ist im Reporting verfügbar.

\### Anwender Feedback Capterra

!!! notice ""

   Wird nur durchgeführt wenn es dazu eine Kampagne gibt.

Positive Bewertungen erhalten im Anschluss außerdem einen manuell versendeten Link auf die Bewertungsplattform "Capterra", bei dem die Anwender synetics bewerten können und bei einer Teilnahme und Abgabe einer validen Bewertung einen 10€ Gutschein erhalten.

\### ZenDesk Pflege und Backup

Das Ticketsystem ist Cloudbasiert gehostet. Updates und Sicherheitsverfahren werden vom Anbieter gestellt.

Ein geregeltes lokales Backup wird seitens des Hosters nicht gestellt. Es gibt die Möglichkeit, ein CSV/XML Backup zu aktivieren. Dieses wird unregelmäßig manuell ausgeführt.

\### Emergency Bug Handling

Wird von uns oder einem Anwender ein Fehler erkannt der als "Emergency BUG" klassifiziert wird, gilt es die hier beschriebenen Schritte einzuhalten.

\_Ein Emergency Bug weist mindestens eins der folgenden Merkmale auf:\_

\- führt potenziell zu der Veränderung oder dem Verlust von Daten aus der Dokumentation in i-doit pro

\- macht eine oder mehrere Kernfunktionen in i-doit pro eingeschränkt bis schwer nutzbar, vitale Funktionen sind gestört, eine Nutzung ist nicht mehr möglich

\- führt zu sicherheitsrelevanten Problemen, der gesicherte Zugriff auf die hinterlegten Daten ist gestört oder der Schutz vor unerwünschtem Zugriff ist nicht mehr gewährleistet

\- führt zu einem Imageschaden für synetics oder das Unternehmen (Anwender)

\- wird zu einem Emergency Bug aus strategischen Gründen definiert, Eskalations-Entscheidungsrecht von GF, Sales oder Partner Manager wird wahrgenommen

Wird eines oder mehrere dieser Merkmale erkannt geht die Eskalation des gemeldeten oder durch uns erkannten Fehlers in ein Entscheidungsrunde mit Care, Produkt und Entwicklung wo eine abschließende Bewertung der Schwere des Fehlers stattfindet.

\---

\## Entscheidungsrunde

Die Entscheidungsrunde entscheidet über die weiteren Schritte betreffend Lösungs/Hot-Fix Entwicklung, Kommunikationsstrategie sowie weiterer organisatorischer Schritte:<br>

Wird hier entschieden dass es sich bei dem Fehler um keinen Emergency Bug handelt wird der Fehler im Rahmen des normalen Bug Handling Prozesses verarbeitet.

Wird hier jedoch zugestimmt und eine klassifizierung als Emergency Bugs bestätigt müssen Entscheidungen für die folgenden Schritte getroffen werden:

\- Kommunikationsstrategie

\- Entwicklung/ Emergency Hot Fix

\- Umfang Testing

\- organisatorische Schritte

\### Kommunikationsstrategie

In der Entscheidungsrunde wird die schwere und die Auswirkung des Bugs bewertet und der für den Bug angemessenen Kommunikationsweg, Umfang und Zeitpunkt definiert.

Es kann entschieden werden, dass sofort, bevor ein Hotfix oder eine Lösung bereitsteht, eine Information an alle oder betroffene Kunden rausgeht, dies kann aktiv per Mail oder als Hinweis im Support Center und in der KB erfolgen.

Diese Meldung sollte folgende Informationen über den Fehler beinhalten:

\- Ursache

\- Auswirkungen

\- Handlungsanweisungen

\- ungefähres Zeitfenster bis zur Bereitstellung eine Lösung/ eines Hotfixes

Es kann aber auch entschieden werden dass erst eine Kommunikation gestartet wird sobald wir eine valide, getestete und dokumentierte Lösung oder einen Hotfix vorliegen haben, auch hier sollten folgende Informationen bereitgestellt werden:

\- Ursache

\- Auswirkungen

\- Lösungsansatz/ Anleitung zur Behebung

\- Nennung des Kommunikations Rückkanals für Fragen/Support

\- Links zur Dokumentation oder weiteren Informationen

Alle Aktionen im Bereich der Kommunikation werden transparent an die beteiligten Abteilungen Care/Produkt/ Entwicklung/Sales und Partnermanagement gespiegelt und über die Strategie im Umgang sowie das offizielle Wording informiert.

\### Entwicklung/ Emergency Hot Fix

Wird in der Entscheidungsrunde der Fehler als Emergency Bug bestätigt startet parallel zu der Kommunikation und den organisatorischen Schritten die Entwicklung einer Lösung.<br>

Je nach festgelegter Priorität und schwere des Fehlers hat die Entwicklung und Bereitstellung vorrang vor anderen aktuellen Themen.

Aus der Entwicklung muss möglichst zeitnah eine ungefähre Einschätzung des Problems und ein zeitlicher Lösungshorizont geliefert werden, diese Information geht, sobald vorhanden, an das Care Team.

Sobald eine Lösung oder ein Hotfix erarbeitet wurde, wird dieser an das Testing zur Verifizierung geliefert. Der Umfang des zu betreibenden Testingaufwands wird in der Entscheidungsrunde getroffen, nach Bereitstellung des Hotfixes aber noch einmal zusammen mit der Entwicklung hinterfragt:

\- Formales, oberflächliches Testen durch Care

\- Durchführung von definierten Tests durch Testing

\- Herausgabe an ausgewählte Kunden zum Testen

\### Organisatorische Schritte

Parallel zu den oben genannten Schritten muss entschieden werden, welche organisatorischen Schritte zur weiteren Behandlung des Bugs angemessen sind:

\- Kommunikation intern oder an Partner

\- entfernen eines fehlerhaften Releases aus dem Portal und anderen Quellen

\- Ressourcenanpassung für Support oder Entwicklung

\- Alle getroffenen Entscheidungen und (Zwischen-)Schritte sowie der aktuelle Stand sind im Ticket nachzuhalten

\---

\## Kommunikation intern oder an Partner

Alle am Prozess beteiligten Personen sollten jederzeit auf dem aktuellen Stand gehalten werden und wissen in welcher Form die Außenkommunikation darüber stattfindet.<br>

Es ist zu entscheiden, ob auch Partner mit ins Boot geholt werden sollen.

\*\*Entfernen eines fehlerhaften Releases aus dem Portal und anderen Quellen\*\*<br>

Es ist zu entscheiden ob der Zugriff auf ein fehlerhafte Release genommen werden soll in dem es aus dem Kundenportal oder anderen Quellen entfernt wird.

\*\*Ressourcenanpassung für Support oder Entwicklung\*\*<br>

Ist damit zu rechnen dass die Auswirkungen zu einem erhöhten Supportaufkommen führen werden sind die entsprechenden Ressourcen pro aktiv zu aktivieren.

\## Arbeitszeiten

Wer 1st Level Dienst hat, muss bis 18 Uhr arbeiten. Daraus folgt eine Arbeitszeit von 09:30 - 18:00 mit 30 Minuten Pause

Für die anderen gilt spätestens um 09:00 Uhr anzufangen, da ab dann der Support besetzt sein muss.