# Pronterface: How to Download, Install & Set It Up - All3DP

Quelle: [Pronterface: How to Download, Install & Set It Up - All3DP](https://all3dp.com/2/pronterface-how-to-download-install-and-set-it-up/ "")

Want more control of your printer? Read along as we download and install Pronterface. You'll be giving immediate commands in no time!

Pronterface is a simple graphical user interface that allows you to monitor and control your printer from a USB-connected computer. 
With it you can directly move stepper motors, control bed and nozzle temperatures, send [G-code](https://all3dp.com/topic/G-code/ "") commands directly via a terminal or console window, and much more.

Created by the influential [RepRap](https://reprap.org/wiki/RepRap "") initiative, Pronterface has been around for a long time, and it’s part of the Printrun suite of simple tools for managing and controlling both 3D printers and CNC machines.

Updated in early 2021, the program runs on Windows, Mac, and Linux machines. 
Despite a fairly basic-looking design, with the bare minimum in graphics, it’s a very useful tool that retains a strong position in the 3D printing community.

In this article, we’ll take a closer look at what Pronterface is, its uses, and how to install and run it.  


## Why Use It?

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121159/the-pronterface-dashboard-reprap-wiki-211102_download-1.jpg)  
The Pronterface Dashboard (Source: [RepRap Wiki](https://reprap.org/wiki/Printrun))  

Originally designed to control the end-to-end 3D printing workflow, including slicing (using Slic3r), Pronterface tends to fulfil a simpler role today. Yet, despite other software options, including OctoPrint and various “G-code senders”, providing much of the same functionality, Pronterface has several distinct advantages.

In addition to running on multiple computer platforms, it’s simple to install, easy to learn (at least for the basic functionality), can be quickly customized to automate repetitive tasks, and is written in Python, allowing more technical users to make their own modifications.

Pronterface has a dedicated website and its own section on the RepRap wiki. However, because of its long heritage and various spin off projects, downloading and installing what you need has the potential to be a little confusing.

We’ve set out what you need to know below.

## Downloading  

![](https://i.all3dp.com/workers/images/fit=cover,w=1000,gravity=0.5x0.5,format=auto/wp-content/uploads/2021/12/22121202/click-the-highlighted-option-above-to-find-the-lat-pronterface-211222_download.jpg)  
Click on the highlighted option as seen above to find the latest Pronterface release (Source: [Pronterface](http://www.pronterface.com/#download)) 


The best starting point to download Pronterface is the [Pronterface website](http://www.pronterface.com/). 
This is actually the home of the entire [PrintRun suite](https://reprap.org/wiki/Printrun) of utilities, which includes Pronterface.

Don’t be distracted by potentially confusing references to previous versions. The most up-to-date software can be found by clicking on the Download tab and then on the “Latest release” link, as seen in the image above.

This will take you to a GitHub page at the foot of which are links to pre-packaged software for MacOS and Windows versions. There are also links to the source code as well as “master tarballs” for those wanting to make their own modifications or install it on Linux. 

## Installation


![]()

The latest Pronterface assets on GitHub (Source: GitHub)
At the time of writing, the version number (for all of the Printrun suite) is  2.0.0rc8.

### Windows
If you’re running Windows, download the correct (64- or 32-bit) zip file, extract the contents to the desired location, and you should be ready to go!

However, depending on the security settings implemented on your computer, you may need to grant explicit permission for the program to run. You may also find that you need to plug in your printer before you first run the software, to give it a better chance of finding the right COM port.

Use Windows Device Manager to check which COM port has been assigned to your 3D printer – you’ll need this during setup. 
If your printer connection isn’t visible or you get a device driver error, then either use Windows “find driver” functionality or visit the source of additional drivers that’s correct for your printer or its controller board. 
([FTDI drivers](https://ftdichip.com/drivers/) is a common source of solutions for 3D printers.)

By this stage, you should be ready to move onto setup.

### MacOS
To install on a Mac, download the “pronterface-macos-app” zip file and unpack it.

By default, the Gatekeeper security feature in MacOS will reject Pronterface, as it hasn’t been explicitly “notarized” for use by Macs. To run it, you’ll need to go to Settings, choose “Security & Privacy”, select the “General” tab, and explicitly allow it to run.

As with Windows machines, recognizing a 3D printer’s USB port can in some cases be problematic. 
Your printer should show up as “/usbmodem port” or something similar. If not, check that the correct drivers are installed (refer to sources like [FTDI drivers](https://ftdichip.com/drivers/) to help). 
If your Mac has had other USB devices plugged into the same physical ports previously, you may also need to reboot. 


### Linux
Full instructions on Linux installs are provided in the Printrun2.x [README.md](https://github.com/kliment/Printrun/blob/master/README.md).

In theory, any Linux device with the appropriate Python installation should be able to run Pronterface, although this will depend on the physical build. 
There are case examples for installation on Ubuntu/Debian, Fedora, Chrome OS, Archlinux, and even [Raspbian](https://all3dp.com/2/noobs-vs-raspbian-difference/) on a [Raspberry Pi](https://all3dp.com/2/what-is-a-raspberry-pi/) (for which there’s a dedicated [Instructable](https://www.instructables.com/How-to-Control-a-3D-Printer-Via-Raspbery-Pi2/), although you may need to update the Python references).

The Linux instructions may also help those modifying the source code to run on Windows or Mac devices.

In all cases, obviously, you’ll need the latest version of Python pre-installed, too.