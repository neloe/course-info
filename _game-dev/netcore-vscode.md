---
title: Visual Studio Code and .NET Core
category: defunct
layout: default
---

## Why Visual Studio Code and .NET Core?

In roughly 2018, Unity removed the integrated MonoDevelop editor for C# Scripts.
The UnityHub installer will Download and Install Visual Studio Community 2019, but I have found that it is a very heavy solution that is somewhat slow, and I never got autocomplete working quite right.
Visual Studio Code seems to be lighter weight and faster, and has several plugins that make the development process easier.

You are not limited to VS Code; you could use any text editor you wanted (Notepad, anyone?), but the autocomplete and syntax highlighting of a programmer's text editor is preferred

Much of this information is taken from [here](https://code.visualstudio.com/docs/other/unity)

## Installer Links

_Note_ If you use the chocolatey package manager both .NET Core and VS Code are available as packages (`dotnetcore-sdk` and `vscode`, respectively)

Make sure you obtain the version for your specific operating system (student laptops use Windows x64, or 64 bit)

* [.NET Core](https://dotnet.microsoft.com/download/dotnet-core)
* [Visual Studio Code](https://code.visualstudio.com/)

### Changing Your Preferred Editor

In Unity itself (once you have a project open) you can change the editor to whatever you want it to be by going to the preferences window.

![Setting VS Code]({{ "assets/img/vscode/set-editor.gif" | relative_url }})
### Visual Studio Code Extensions
