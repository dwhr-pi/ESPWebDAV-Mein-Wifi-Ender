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


## Downloading  

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121202/click-the-highlighted-option-above-to-find-the-lat-pronterface-211222_download.jpg)  
Click on the highlighted option as seen above to find the latest Pronterface release (Source: [Pronterface](http://www.pronterface.com/#download)) 


The best starting point to download Pronterface is [the Pronterface website](http://www.pronterface.com/). 
This is actually the home of the entire [PrintRun](https://reprap.org/wiki/Printrun) suite of utilities, which includes Pronterface.

Don’t be distracted by potentially confusing references to previous versions. The most up-to-date software can be found by clicking on the Download tab and then on the “Latest release” link, as seen in the image above.

This will take you to a GitHub page at the foot of which are links to pre-packaged software for MacOS and Windows versions. There are also links to the source code as well as “master tarballs” for those wanting to make their own modifications or install it on Linux. 



## Installation
![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121207/latest-pronterface-assets-on-github-github-211222_download-e1640176008641.jpg)

The latest Pronterface assets on GitHub (Source: [GitHub](https://github.com/kliment/Printrun/releases/tag/printrun-2.0.0rc8))
At the time of writing, the version number (for all of the Printrun suite) is  2.0.0rc8.

### Windows
If you’re running Windows, download the correct (64- or 32-bit) zip file, extract the contents to the desired location, and you should be ready to go!

However, depending on the security settings implemented on your computer, you may need to grant explicit permission for the program to run. You may also find that you need to plug in your printer before you first run the software, to give it a better chance of finding the right COM port.

Use Windows Device Manager to check which COM port has been assigned to your 3D printer – you’ll need this during setup. 
If your printer connection isn’t visible or you get a device driver error, then either use Windows “find driver” functionality or visit the source of additional drivers that’s correct for your printer or its controller board. 
([FTDI drivers](https://ftdichip.com/drivers/) is a common source of solutions for 3D printers.)

By this stage, you should be ready to move onto setup.

### MacOS
![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121210/you-can-find-the-whole-printrun-package-for-your-o-github-211222_download-e1640176039700.jpg)  
You can find the whole Printrun package for your OS (Source: [GitHub](https://all3dp.com/2/pronterface-how-to-download-install-and-set-it-up/#:~:text=You%20can%20find%20the%20whole%20Printrun%20package%20for%20your%20OS%20(Source%3A%20GitHub)))  

To install on a Mac, download the “pronterface-macos-app” zip file and unpack it.

By default, the Gatekeeper security feature in MacOS will reject Pronterface, as it hasn’t been explicitly “notarized” for use by Macs. 
To run it, you’ll need to go to Settings, choose “Security & Privacy”, select the “General” tab, and explicitly allow it to run.

As with Windows machines, recognizing a 3D printer’s USB port can in some cases be problematic. 
Your printer should show up as “/usbmodem port” or something similar. If not, check that the correct drivers are installed (refer to sources like [FTDI drivers](https://ftdichip.com/drivers/) to help). 
If your Mac has had other USB devices plugged into the same physical ports previously, you may also need to reboot. 


### Linux
Full instructions on Linux installs are provided in the Printrun2.x [README.md](https://github.com/kliment/Printrun/blob/master/README.md).

In theory, any Linux device with the appropriate Python installation should be able to run Pronterface, although this will depend on the physical build. 
There are case examples for installation on Ubuntu/Debian, Fedora, Chrome OS, Archlinux, and even [Raspbian](https://all3dp.com/2/noobs-vs-raspbian-difference/) on a [Raspberry Pi](https://all3dp.com/2/what-is-a-raspberry-pi/) (for which there’s a dedicated [Instructable](https://www.instructables.com/How-to-Control-a-3D-Printer-Via-Raspbery-Pi2/), although you may need to update the Python references).

The Linux instructions may also help those modifying the source code to run on Windows or Mac devices.

In all cases, obviously, you’ll need the latest version of Python pre-installed, too. 


## Setup

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121214/part-of-the-pronterface-setup-menus-ken-douglas-via-all3dp-211102_download-e1640175810953.jpg)  
Part of the Pronterface Settings menu (Source: Ken Douglas via All3DP)  

There are a few setup and configuration tasks to complete at this stage. First, select the port to which the printer is connected. On Windows, this will be something like COM8, while on a Mac, it will typically be a variant of “/usbmodem” or “/tty”. If these are not present, refer to the points about USB drivers and connections in the section above.

Next check the communications speed. The default of 115200 is usually the best, but may vary according to your printer.

At this stage, you can click connect and see a message confirming that Pronterface and your 3D printer are communicating. You will then be able to use the basic controls and also send G-code commands via the terminal. (See the section below.)

Depending on the tasks you have in mind, you may need to further configure Pronterface so that it knows more about your printer. Do this by selecting the “Settings” menu option and then “Options” from the dropdown list. This will present a menu window with several tabs covering Printer settings, User interface, and more. 90% of the time, these do not need to altered.  

## Operation

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121217/getting-to-know-the-layout-wardsci-211102_download.jpg)
Getting to know the layout (Source: [Wardsci](https://www.wardsci.com/assetsvc/asset/en_US/id/24203892/contents))  

Although Pronterface can open and handle both [STL](https://all3dp.com/1/stl-file-format-3d-printing/) and G-code files, it’s slow compared to a modern slicer and other tools that send G-code commands (such as OctoPrint). 
These days, therefore, its use is more focused on testing, configuration, calibration, and related tasks.

Although some printers have built-in terminals to allow G-code to be entered and executed directly, Pronterface is usually quicker and easier. 
Plenty of recent [YouTube videos](https://www.youtube.com/watch?v=T1TH0QpHVWs) on Pronterface tend to focus on this type of usage.

Layout
The following are the different parts of Pronterface (as seen above):

- A: Port Selection
- B: Control Panel
- C: Heater Control
- D Extruder Control
- E: Custom Button Area
- F: Command Line
- G: Command Window


## Printer Control & Simple G-code Commands
The simple graphical interface makes it easy to control the basic features of a 3D printer, while other tasks require G-code commands to be typed in directly. 
This is a great way to [learn about G-code](https://all3dp.com/2/easy-g-code-examples-to-begin-with/).

More experienced users may make use of advanced commands supported by whatever firmware their printer runs, such as the [extensive list](https://marlinfw.org/meta/gcode/) supported by [Marlin]().

## Custom Options 
A particularly useful feature of Pronterface is the ability to quickly set up custom buttons that can store and automate frequently used G-code tasks. 
To do this, click the “+” icon in the Custom Button Area, enter a name, the G-code commands, and specify a color for the button. 
(Hint: the colors are specified using the [hex standard](https://htmlcolorcodes.com/).)

These can be used for extruding specific lengths of filament, selectively enabling and disabling stepper motors, switching software endstops on and off, reporting saved configuration settings, moving to specified positions, switching peripherals (such as filament sensors) on and off, and much more.

There are other G-code senders available, but few can be as universally deployed as Pronterface or have the potential to be tailored or modified for a variety of applications as this program.

![]()

![]()