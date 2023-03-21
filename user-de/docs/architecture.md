## System-Architektur

Das *imperia* CMS besteht im Wesentlichen aus zwei Systemen: dem Basissystem (historische Synonyme: Developsystem) und den Zielsystemen (historische Synonyme: Livesysteme).

Das Entwicklungsystem ist Teil von *imperia*, und ermöglicht Autoren Dokumente zu erstellen und zu bearbeiten. Welche Aktionen durch Autoren in den Dokumenten durchgeführt werden können, ist hauptsächlich abhängig von den Rollen und Workflows, die im Entwicklungsystem definiert sind.

Ist die Arbeit an einem Dokument erledigt, wird es, entweder manuell oder automatisch, vom Basissystem auf die Zielsysteme übertragen. Diesen Vorgang nennt man *freischalten*. Das Freischalten geschieht über Freischalt-Plug-ins, mit deren Hilfe verschiedene Zielformate auf dem Zielsystem erzeugt werden können. Verwendet man das HTML-Freischalt-Plug-in, so kopiert *imperia*  die schon auf dem Basissystem im Filesystem abgelegten und über Templates generierten Dokumente in das Filesystem des entsprechenden Zielsystems. Aus diesen freigeschalteten Dokumenten kann das Zielsystem automatisch Übersichtsseiten generieren und so dafür sorgen, dass diese immer einen aktuellen Überblick über die Themen des Webauftritts bieten. Diese Aufgabe übernimmt *SiteActive* in Zusammenarbeit mit dem Hintergrund-Daemon *Hermes* und dem Notification-Freischalt-Plug-in. Durch dieses Notification-Plug-in werden alle Metainformationen eines Dokumentes in einem Binärformat auf das Zielsystem kopiert. Der Hintergrund-Daemon *Hermes* verarbeitet dieses Notification-File und legt auf dem Zielsystem der *imperia-*Installation eine Datenhaltung an. Zusätzlich werden über das Notification-File die sogenannten Systemdienste getriggert, die die oben erwähnten *SiteActive*-Funktionen steuern.

Seit seiner Einführung 1995 hat sich das Produkt *imperia*  durch intensive Zusammenarbeit mit Kunden und Endanwendern zu einem Standardprodukt für Website- und Content-Management entwickelt. Neben zahlreichen großen Installationen mit Millionen von Seitenaufrufen pro Tag hat *imperia*  auch bei mittelständischen Betrieben und Startups seine Flexibilität und Leistungsfähigkeit unter Beweis gestellt. Alle *imperia-*Module weisen folgende Gemeinsamkeiten auf:

* Sie sind plattformunabhängig.

* Es wird keine zusätzliche Client-Software benötigt; die Bedienung erfolgt ausschließlich im Web-Browser.

* Alle *imperia-*Module werden im Source-Code ausgeliefert.

* Module sind skalierbar und modular und somit leicht erweiterbar.

* Die Verwendung von einzelnen Modulen wird durch Benutzer- und Rollenberechtigungen gesteuert.

* Die Daten werden in einem File-System oder in einer Datenbank gespeichert.


