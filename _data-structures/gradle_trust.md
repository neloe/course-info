---
title: Resolving the Project Problems Dialog in NetBeans + Gradle
layout: default
category: software
---

The first time you open each project in NetBeans, you may be greeted with this dialog box:

![Project Problems]({{ "assets/img/gradle/need_priming.png" | relative_url }})

This appears because NetBeans needs to execute what is known as a "priming build" to resolve project dependencies.

If you close this window, you can fix it by clicking the "build" icon in the toolbar (![Build Icon](img/gradle/build.png)), but we can configure NetBeans to automatically trust projects as we open them.

First, open the Tools menu and go to Options.
You should be greeted with a window with several different configuration possibilities.
Choose the "Java" tab.

![Options Dialog]({{ "assets/img/gradle/opts_java.png" | relative_url }})

In this tab, you will want to choose the "Gradle" tab (highlighted in the image above).
Towards the bottom of this page (under the "Execution" category) you should see an option for "Allow Gradle Execution" (highlighted below)

![Gradle Options]({{ "assets/img/gradle/opts_gradle.png" | relative_url }})

In the dropdown menu, select "Always", then hit the "Apply" button at the bottom of the options dialog.
From now on, when you first open a project from this class in NetBeans, you should not see that Project Problems dialog box!
