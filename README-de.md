## WebDAV-Server und ein 3D-Drucker
Dieses Projekt ist ein WiFi-WebDAV-Server mit ESP8266 SoC. Es verwaltet das Dateisystem auf einer SD-Karte.

Unterstützt die grundlegenden WebDav-Operationen - *PROPFIND*, *GET*, *PUT*, *DELETE*, *MKCOL*, *MOVE* usw.

Sobald der WebDAV-Server auf dem ESP8266 läuft, kann ein WebDAV-Client wie Windows wie auf ein Cloud-Laufwerk auf das Dateisystem auf der SD-Karte zugreifen.
Das Laufwerk kann auch wie ein Netzwerklaufwerk gemountet werden und ermöglicht das Kopieren/Einfügen/Löschen von Dateien auf der SD-Karte aus der Ferne. 

### 3D Drucker

Ich verwende dieses Setup als Netzwerklaufwerk für 3D-Drucker mit Marlin. Die folgende Schaltung mit ESP8266 und einem MicroSD-Adapter wird auf einer Leiterplatte hergestellt.
Ein SD-Kartenadapter in voller Größe wird an ein Ende geklebt und bietet Zugriff auf alle SPI-Datenleitungen vom Drucker. 
Der ESP8266-Code vermeidet den Zugriff auf die Micro-SD-Karte, wenn Marlin (Drucker-Firmware) darauf liest/schreibt (erkannt über die Chip-Select-Leitung).  

GCode kann direkt vom Slicer (Cura) auf dieses Remote-Laufwerk hochgeladen werden, wodurch der Arbeitsablauf vereinfacht wird.

![Printer Hookup Diagram](PrinterHookup2.jpg)

## Abhängigkeiten:  
1. [ESP8266 Arduino Core version 2.4](https://github.com/esp8266/Arduino)
2. [SdFat library](https://github.com/greiman/SdFat)
  

## Verwenden:
Kompilieren Sie das Programm und laden Sie es in ein ESP8266-Modul hoch. ESP12-E wurde für Entwicklung und Tests verwendet.
Verbinden Sie die SPI-Busleitungen mit der SD-Karte.  


ESP Module|SD Card
---|---
GPIO13|MOSI   
GPIO12|MISO   
GPIO14|SCK    
GPIO4|CS   
GPIO5|CS Sense   

Die Karte sollte für Fat16 oder Fat32 formatiert sein.  

Um von Windows aus auf das Laufwerk zuzugreifen, geben Sie  in der Eingabeaufforderung „Ausführen“ ```\\esp_hostname_or_ip\DavWWWRoot``` ein oder verwenden Sie das Menü „Netzlaufwerk verbinden“ im Windows Explorer.

## Verweise
Marlin Firmware - [http://marlinfw.org/](http://marlinfw.org/)   

Cura Slicer - [https://ultimaker.com/en/products/ultimaker-cura-software](https://ultimaker.com/en/products/ultimaker-cura-software)   

3D Printer LCD and SD Card Interface - [http://reprap.org/wiki/RepRapDiscount_Full_Graphic_Smart_Controller](http://reprap.org/wiki/RepRapDiscount_Full_Graphic_Smart_Controller)   

LCD Schematics - [http://reprap.org/mediawiki/images/7/79/LCD_connect_SCHDOC.pdf](http://reprap.org/mediawiki/images/7/79/LCD_connect_SCHDOC.pdf)   



## Das Video ist auf Youtube
[YouTube: SD Card + ESP8266 = OctoPrint Alternative?](https://www.youtube.com/watch?v=nHNZPRl8gzA&t=620s "") bei 5:54 beschreibt `Thomas Sanladerer` das WiFi-Setup. 
Er verwendet dazu: [FYSETC/ESPWebDAV](https://github.com/FYSETC/ESPWebDAV "") und dies stellt einen Clone vom Original [ardyesp/ESPWebDAV](https://github.com/ardyesp/ESPWebDAV "") da.



Ab 6:20 min. beschreibt er, das er dazu [Pronterface](https://www.google.com/search?q=pronterface+download&oq=Pronterface&aqs=chrome.1.69i57j0i512l9.3406j0j7&sourceid=chrome&ie=UTF-8 "") und dies ist eine [Pronterface: Printrun: Pure Python 3d printing host software](https://www.pronterface.com/ "") verwendet. 
Für Pronteface gibt es eine weitere Beschreibung [Pronterface: How to Download, Install & Set It Up - All3DP](https://all3dp.com/2/pronterface-how-to-download-install-and-set-it-up/ "").


![SD-WIFI with Card-Reader Module ESP8266 USB to serial Wireless Transmission NEW](assets/s-l500.jpg)  
[Ebay: SD-WIFI with Card-Reader Module ESP8266 USB to serial Wireless Transmission NEW](https://www.ebay.de/itm/265689753420?_trkparms=amclksrc%3DITM%26aid%3D777008%26algo%3DPERSONAL.TOPIC%26ao%3D1%26asc%3D20220822113838%26meid%3Dc43b115613e1420491e2ab98faffd084%26pid%3D101524%26rk%3D1%26rkt%3D1%26sd%3D122891034180%26itm%3D265689753420%26pmt%3D0%26noa%3D1%26pg%3D2380057%26algv%3DRecentlyViewedItemsV2%26brand%3DMarkenlos&_trksid=p2380057.c101524.m146925&_trkparms=pageci%3A42190337-7bd1-11ed-94b4-6a2cf1bac2ca%7Cparentrq%3A119783e41850aa702763a77dfff8a302%7Ciid%3A1)  
Preis: EUR 16,64 (inkl. MwSt.)  

![SD-WIFI with Card-Reader Module ESP8266 USB to serial Wireless Transmission NEW](assets/s-l500(1).jpg)  
[Ebay: SD-WIFI with Card-Reader Module ESP8266 USB to serial Wireless Transmission NEW](https://www.ebay.de/itm/234550269364?_trkparms=amclksrc%3DITM%26aid%3D777008%26algo%3DPERSONAL.TOPIC%26ao%3D1%26asc%3D20220822113838%26meid%3Dc43b115613e1420491e2ab98faffd084%26pid%3D101524%26rk%3D1%26rkt%3D1%26sd%3D122891034180%26itm%3D234550269364%26pmt%3D0%26noa%3D1%26pg%3D2380057%26algv%3DRecentlyViewedItemsV2%26brand%3DMarkenlos&_trksid=p2380057.c101524.m146925&_trkparms=pageci%3A42190337-7bd1-11ed-94b4-6a2cf1bac2ca%7Cparentrq%3A119783e41850aa702763a77dfff8a302%7Ciid%3A1)  
Preis: EUR 16,79 (inkl. MwSt.)  

## Product Description

### Introduction

Das SD-WIFI ist ein Modul, das ESPwebDev （https://github.com/ardyesp/ESPWebDAV） ausführen kann. 
Wir haben es in Form einer SD-Karte gestaltet, sodass es direkt in einen vorhandenen SD-Kartensteckplatz eingesetzt und mit Strom versorgt werden kann.
Sie können es mit dem von uns bereitgestellten seriellen Befehl mit dem Router verbinden und dann die zurückgegebene IP-Adresse notieren.
Dann kann ein WebDAV-Client wie Windows auf das Dateisystem auf der SD-Karte wie auf eine Cloud-Festplatte zugreifen und entfernt Befehle wie: replication / Paste / delete Dateien auf der SD-Karte zu lassen.  

Wenn Sie eine Flash-Air-SD-Karte für Toshiba verwendet haben, sollten Sie diese Methode verstehen.
Flash-Air kann jedoch nicht mit dem Router verbunden werden, da es als AP ausgeführt wird und nur ein Gerät damit verbunden werden kann.
Wenn beispielsweise Ihr Computer damit verbunden ist, können Sie sich nicht mehr gleichzeitig mit dem Internet verbinden.
Unser Modul wird jedoch als Client für den Zugriff auf das LAN verwendet, und alle Geräte im Netzwerk können darauf zugreifen, ohne die ursprüngliche Verbindung zu beeinträchtigen.  
 
### Summary
 

Operating Voltage: 3.3V（Via SD Finger ）/5V（Via USB）
USB to serial chip: CH340E
Max Current: 600mA
Size: 49.5mm x 24mm
Feature

On-board SD card reader (for card reading via USB)
Onboard USB to serial chip (used for wifi configuration via serial port)
USB toggle switch (between card reader and serial chip)
3.3V 600mA LDO (used when WIFI module power supply is plugged in USB)
 
 
Package Included: 1pcs 


Guarantee

1. 12 months Manufacturer’s limited Warranty for defective items (excluding items damaged and/or misused after receipt). Accessories come with a 3-month warranty.
2. Defective items MUST BE reported and returned within the warranty period (and in the original packaging, if possible). You must tell us what the defect is and give us your order number. 
WE DO NOT REPAIR OR REPLACE ITEMS WITH AN EXPIRED WARRANTY.