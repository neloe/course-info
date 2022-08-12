---
title: Installing the JDK and Apache Netbeans
layout: default
category: software
---

## Getting the JDK

Go to [Adoptium](https://adoptium.net)

Download the Latest LTS release for your computer and OS (student laptops are Windows x64, or 64 bit Windows)

Run the downloaded installer.  You will reach a screen that looks like this:

![JDK Option Selection]({{ "assets/img/jdk_nb/option_choose.PNG" | relative_url }})

Select the drop down next to `Set JAVA_HOME variable` and choose "Will be installed on local hard drive".
Continue on to finish the installation.

## Apache Netbeans

Download the newest version of [Apache Netbeans](https://netbeans.apache.org/download/index.html).
At the time of writing this page, the newest version is [14](https://netbeans.apache.org/download/nb14/nb14.html).
Make sure you download the installer for your system, and run it.

One screen of the installer gives you an option for the specific JDK to use; make sure it points to the Java SDk you installed previously (the path will be similar to the below image; on my latest install the path was `C:\Program Files\Eclipse Adoptium\jdk-17.0.4.8-hotspot`).

![AdoptOpenJDK Path]({{ "assets/img/jdk_nb/select_jdk.PNG" | relative_url }})

Finish the installation process.

### Installing the nb-javac plugin

The first time you open a project in Netbeans 12, you may see a window that looks like this:

![NB Javac]({{ "assets/img/jdk_nb/netbeans-nbjavac.PNG" | relative_url }})

Follow through the prompts to install the `nb-javac` editing support library (and the JavaFX Implementation for Windows).
