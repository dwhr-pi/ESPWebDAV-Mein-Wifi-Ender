# Pronterface: Herunterladen, Installieren und Einrichten – All3DP

Quelle: [Pronterface: Anleitung zum Herunterladen, Installieren und Einrichten – All3DP](https://all3dp.com/2/pronterface-how-to-download-install-and-set-it-up/ "")

Möchten Sie mehr Kontrolle über Ihren Drucker? Lesen Sie mit, während wir Pronterface herunterladen und installieren. Sie werden in kürzester Zeit sofortige Befehle erteilen!

Pronterface ist eine einfache grafische Benutzeroberfläche, mit der Sie Ihren Drucker von einem über USB angeschlossenen Computer aus überwachen und steuern können.
Damit können Sie Schrittmotoren direkt bewegen, Bett- und Düsentemperaturen steuern, [G-Code](https://all3dp.com/topic/G-code/ "") Befehle direkt über ein Terminal- oder Konsolenfenster senden und vieles mehr mehr.

Pronterface wurde von der einflussreichen [RepRap](https://reprap.org/wiki/RepRap "")-Initiative entwickelt, gibt es schon seit langer Zeit und ist Teil der Printrun-Suite mit einfachen Tools zur Verwaltung und Steuerung beider 3D-Drucker und CNC-Maschinen.

Das Programm wurde Anfang 2021 aktualisiert und läuft auf Windows-, Mac- und Linux-Computern.
Trotz eines ziemlich einfach aussehenden Designs mit dem Nötigsten an Grafiken ist es ein sehr nützliches Werkzeug, das eine starke Position in der 3D-Druck-Community behält.

In diesem Artikel werden wir uns genauer ansehen, was Pronterface ist, wie es verwendet wird und wie es installiert und ausgeführt wird.


## Warum verwenden?

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121159/the-pronterface-dashboard-reprap-wiki-211102_download-1.jpg)  
Das Pronterface Dashboard (Quelle: [RepRap Wiki](https://reprap.org/wiki/Printrun))  

Pronterface wurde ursprünglich entwickelt, um den End-to-End-3D-Druck-Workflow zu steuern, einschließlich Slicing (unter Verwendung von [Slic3r](https://all3dp.com/2/what-is-slic3r-simply-explained/)), und erfüllt tendenziell a heute eine einfachere Rolle.
Doch trotz anderer Softwareoptionen, einschließlich [OctoPrint](https://all3dp.com/2/octoprint-setup-how-to-install-octopi-on-a-raspberry-pi/) und verschiedener "G-Code-Sender", bietet Pronterface im Wesentlichen die gleiche Funktionalität, hat aber mehrere deutliche Vorteile.

Es läuft nicht nur auf mehreren Computerplattformen, es ist einfach zu installieren, leicht zu erlernen (zumindest für die Grundfunktionen), kann schnell angepasst werden, um sich wiederholende Aufgaben zu automatisieren, und ist in Python geschrieben, sodass technisch versiertere Benutzer ihre eigenen Änderungen vornehmen können. 

Pronterface hat eine [spezielle Website](http://www.pronterface.com/) und einen eigenen Abschnitt im [RepRap-Wiki](https://reprap.org/wiki/Printrun).
Aufgrund seines langen Erbes und verschiedener Spin-off-Projekte kann das Herunterladen und Installieren dessen, was Sie benötigen, jedoch möglicherweise etwas verwirrend sein.

Wir haben unten aufgeführt, was Sie wissen müssen.


## Herunterladen

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121202/click-the-highlighted-option-above-to-find-the-lat-pronterface-211222_download.jpg)  
Klicken Sie auf die hervorgehobene Option wie oben gezeigt, um die neueste Pronterface-Version zu finden (Quelle: [Pronterface](http://www.pronterface.com/#download))


Der beste Ausgangspunkt zum Herunterladen von Pronterface ist [die Pronterface-Website](http://www.pronterface.com/).
Dies ist eigentlich die Heimat der gesamten [PrintRun](https://reprap.org/wiki/Printrun)-Suite von Dienstprogrammen, einschließlich Pronterface.

Lassen Sie sich nicht durch potenziell verwirrende Verweise auf frühere Versionen ablenken. Die aktuellste Software finden Sie, indem Sie auf die Registerkarte „Download“ und dann auf den Link „Neueste Version“ klicken, wie im Bild oben zu sehen.

Dadurch gelangen Sie zu einer GitHub-Seite, an deren Fuß sich Links zu vorgefertigter Software für MacOS- und Windows-Versionen befinden. Es gibt auch Links zum Quellcode sowie „Master-Tarballs“ für diejenigen, die ihre eigenen Änderungen vornehmen oder unter Linux installieren möchten.

## Installation
![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121207/latest-pronterface-assets-on-github-github-211222_download-e1640176008641.jpg)  

Die neuesten Pronterface-Assets auf GitHub (Quelle: [GitHub](https://github.com/kliment/Printrun/releases/tag/printrun-2.0.0rc8))
Zum Zeitpunkt des Schreibens lautet die Versionsnummer (für die gesamte Printrun-Suite) 2.0.0rc8.

### Windows
Wenn Sie Windows verwenden, laden Sie die richtige (64- oder 32-Bit) ZIP-Datei herunter, extrahieren Sie den Inhalt an den gewünschten Ort, und Sie sollten bereit sein!

Abhängig von den auf Ihrem Computer implementierten Sicherheitseinstellungen müssen Sie dem Programm jedoch möglicherweise ausdrücklich die Erlaubnis erteilen, ausgeführt zu werden. Möglicherweise müssen Sie Ihren Drucker auch anschließen, bevor Sie die Software zum ersten Mal ausführen, um eine bessere Chance zu haben, den richtigen COM-Anschluss zu finden.

Verwenden Sie den Windows-Geräte-Manager, um zu überprüfen, welcher COM-Anschluss Ihrem 3D-Drucker zugewiesen wurde – Sie benötigen diesen während der Einrichtung.
Wenn Ihre Druckerverbindung nicht sichtbar ist oder Sie einen Gerätetreiberfehler erhalten, verwenden Sie entweder die Windows-Funktion „Treiber suchen“ oder besuchen Sie die Quelle zusätzlicher Treiber, die für Ihren Drucker oder seine Steuerplatine geeignet sind.
([FTDI-Treiber](https://ftdichip.com/drivers/) ist eine gängige Quelle für Lösungen für 3D-Drucker.)

Zu diesem Zeitpunkt sollten Sie bereit sein, mit der Einrichtung fortzufahren.


### MacOS
![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121210/you-can-find-the-whole-printrun-package-for-your-o-github-211222_download-e1640176039700.jpg)  
Sie finden das gesamte Printrun-Paket für Ihr Betriebssystem (Quelle: [GitHub](https://all3dp.com/2/pronterface-how-to-download-install-and-set-it-up/#:~:text=You%20can%20find%20the%20whole%20Printrun%20package%20for%20your%20OS%20(Source%3A%20GitHub)))  

Um auf einem Mac zu installieren, laden Sie die ZIP-Datei „pronterface-macos-app“ herunter und entpacken Sie sie.

Standardmäßig lehnt die Gatekeeper-Sicherheitsfunktion in MacOS Pronterface ab, da es nicht explizit für die Verwendung durch Macs „beglaubigt“ wurde.
Um es auszuführen, müssen Sie zu den Einstellungen gehen, „Sicherheit und Datenschutz“ auswählen, die Registerkarte „Allgemein“ auswählen und die Ausführung explizit zulassen.

Wie bei Windows-Maschinen kann das Erkennen des USB-Anschlusses eines 3D-Druckers in einigen Fällen problematisch sein.
Ihr Drucker sollte als „/usbmodem port“ oder ähnlich angezeigt werden. Wenn nicht, überprüfen Sie, ob die richtigen Treiber installiert sind (siehe Quellen wie [FTDI-Treiber](https://ftdichip.com/drivers/) um Hilfe zu erhalten).
Wenn an Ihrem Mac zuvor andere USB-Geräte an denselben physischen Ports angeschlossen waren, müssen Sie möglicherweise auch neu starten.


### Linux
Vollständige Anweisungen zu Linux-Installationen finden Sie in Printrun2.x [README.md](https://github.com/kliment/Printrun/blob/master/README.md).

Theoretisch sollte jedes Linux-Gerät mit der entsprechenden Python-Installation in der Lage sein, Pronterface auszuführen, obwohl dies vom physischen Build abhängt.
Es gibt Fallbeispiele für die Installation unter Ubuntu/Debian, Fedora, Chrome OS, Archlinux und sogar [Raspbian](https://all3dp.com/2/noobs-vs-raspbian-difference/) auf einem [Raspberry Pi](https://all3dp.com/2/what-is-a-raspberry-pi/) (für die es ein dediziertes [Instructable](https://www.instructables.com/How-to-Control-a-3D-Printer-Via-Raspbery-Pi2/) gibt, obwohl Sie möglicherweise die Python-Referenzen aktualisieren müssen).

Die Linux-Anweisungen können auch denjenigen helfen, die den Quellcode für die Ausführung auf Windows- oder Mac-Geräten ändern.

In allen Fällen benötigen Sie natürlich auch die neueste Version von Python vorinstalliert.


## Setup

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121214/part-of-the-pronterface-setup-menus-ken-douglas-via-all3dp-211102_download-e1640175810953.jpg)  
Teil des Pronterface-Einstellungsmenüs (Quelle: Ken Douglas via All3DP)  

In dieser Phase müssen einige Einrichtungs- und Konfigurationsaufgaben ausgeführt werden. Wählen Sie zunächst den Anschluss aus, an dem der Drucker angeschlossen ist. 
Unter Windows ist dies so etwas wie COM8, während es auf einem Mac typischerweise eine Variante von „/usbmodem“ oder „/tty“ ist. Wenn diese nicht vorhanden sind, lesen Sie die Punkte zu USB-Treibern und Anschlüssen im Abschnitt oben.

Als nächstes überprüfen Sie die Kommunikationsgeschwindigkeit. 
Der Standardwert von 115200 ist normalerweise der beste, kann aber je nach Drucker variieren.

In diesem Stadium können Sie auf Verbinden klicken und eine Meldung sehen, die bestätigt, dass Pronterface und Ihr 3D-Drucker kommunizieren.
 Sie können dann die grundlegenden Steuerelemente verwenden und auch G-Code-Befehle über das Terminal senden. (Siehe Abschnitt unten.)

Abhängig von den Aufgaben, die Sie im Sinn haben, müssen Sie Pronterface möglicherweise weiter konfigurieren, damit es mehr über Ihren Drucker weiß. 
Wählen Sie dazu die Menüoption „Einstellungen“ und dann „Optionen“ aus der Dropdown-Liste. Dadurch wird ein Menüfenster mit mehreren Registerkarten für Druckereinstellungen, Benutzeroberfläche und mehr angezeigt. 
In 90 % der Fälle müssen diese nicht geändert werden.


## Operation

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121217/getting-to-know-the-layout-wardsci-211102_download.jpg)
Layout kennenlernen (Quelle: [Wardsci](https://www.wardsci.com/assetsvc/asset/en_US/id/24203892/contents))

Obwohl Pronterface sowohl [STL](https://all3dp.com/1/stl-file-format-3d-printing/) als auch G-Code-Dateien öffnen und verarbeiten kann, ist es langsam im Vergleich zu einem modernen Slicer und anderen sendenden Tools G-Code-Befehle (wie OctoPrint).
Heutzutage konzentriert sich seine Verwendung daher mehr auf das Testen, Konfigurieren, Kalibrieren und verwandte Aufgaben.

Obwohl einige Drucker über eingebaute Terminals verfügen, über die G-Code direkt eingegeben und ausgeführt werden kann, ist Pronterface normalerweise schneller und einfacher.
Viele neuere [YouTube-Videos](https://www.youtube.com/watch?v=T1TH0QpHVWs) zu Pronterface konzentrieren sich in der Regel auf diese Art der Nutzung.

### Layout  
Das Folgende sind die verschiedenen Teile von Pronterface (wie oben zu sehen):

- A: Anschlussauswahl
- B: Bedienfeld
- C: Heizungssteuerung
- D Extrudersteuerung
- E: Benutzerdefinierter Schaltflächenbereich
- F: Befehlszeile
- G: Befehlsfenster


Getting to know the layout (Source: [Wardsci](https://www.wardsci.com/assetsvc/asset/en_US/id/24203892/contents))  

## Druckersteuerung und einfache G-Code-Befehle
Die einfache grafische Benutzeroberfläche erleichtert die Steuerung der Grundfunktionen eines 3D-Druckers, während andere Aufgaben die direkte Eingabe von G-Code-Befehlen erfordern.
Dies ist eine großartige Möglichkeit, [mehr über G-Code zu erfahren](https://all3dp.com/2/easy-g-code-examples-to-begin-with/).

Erfahrenere Benutzer können erweiterte Befehle verwenden, die von der Firmware unterstützt werden, auf der ihr Drucker ausgeführt wird, z. B. die [umfangreiche Liste](https://marlinfw.org/meta/gcode/), die von [Marlin](https://all3dp.com/topic/marlin/) unterstützt wird.

## Benutzerdefinierte Optionen
Eine besonders nützliche Funktion von Pronterface ist die Möglichkeit, schnell benutzerdefinierte Schaltflächen einzurichten, die häufig verwendete G-Code-Aufgaben speichern und automatisieren können.
Klicken Sie dazu auf das „+“-Symbol im Bereich für benutzerdefinierte Schaltflächen, geben Sie einen Namen, die G-Code-Befehle und eine Farbe für die Schaltfläche ein.
(Hinweis: Die Farben werden mit dem [Hex-Standard](https://htmlcolorcodes.com/) angegeben.)

Diese können zum Extrudieren bestimmter Filamentlängen, zum selektiven Aktivieren und Deaktivieren von Schrittmotoren, zum Ein- und Ausschalten von Software-Endstopps, zum Melden gespeicherter Konfigurationseinstellungen, zum Bewegen zu bestimmten Positionen, zum Ein- und Ausschalten von Peripheriegeräten (z. B. Filamentsensoren) und vielem mehr verwendet werden .

Es sind andere G-Code-Sender verfügbar, aber nur wenige können so universell eingesetzt werden wie Pronterface oder haben das Potenzial, für eine Vielzahl von Anwendungen maßgeschneidert oder modifiziert zu werden wie dieses Programm.

