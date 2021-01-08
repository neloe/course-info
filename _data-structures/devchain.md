---
title: Installing the JDK and Apache Netbeans
layout: default
category: software
---

## Getting the JDK

Go to [AdoptOpenJDK](https://adoptopenjdk.net)

Make sure that OpenJDK11 (LTS) and HotSpot are selected, and download the latest release for your computer (student laptops are Windows x64, or 64 bit Windows).

![JDK Version Selection]({{ "assets/img/jdk_nb/jvm_choose.PNG" | relative_url }})

Run the downloaded installer.  You will reach a screen that looks like this:

![JDK Option Selection]({{ "assets/img/jdk_nb/option_choose.PNG" | relative_url }})

Select the drop down next to `Set JAVA_HOME variable` and choose "Will be installed on local hard drive".
Continue on to finish the installation.

## Apache Netbeans

Download the newest version of Apache Netbeans from https://netbeans.apache.org/ .
At the time of writing this page, the newest version is [12.2](https://netbeans.apache.org/download/nb122/nb122.html).
Make sure you download the installer for your system, and run it.

One screen of the installer gives you an option for the specific JDK to use; make sure it points to AdoptOpenJDK11 (the path will be similar to the below image).

![AdoptOpenJDK Path]({{ "assets/img/jdk_nb/select_jdk.PNG" | relative_url }})

Finish the installation process.

### Installing the nb-javac plugin

The first time you open a project in Netbeans 12, you should see a window that looks like this:

![NB Javac]({{ "assets/img/jdk_nb/netbeans-nbjavac.PNG" | relative_url }})

Follow through the prompts to install the `nb-javac` editing support library (and the JavaFX Implementation for Windows).
