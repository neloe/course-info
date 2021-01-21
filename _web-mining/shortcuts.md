---
title: Virtual Environment Shortcuts (Windows)
category: software
layout: default
---

Just running the `jupyter-lab` shortcut leaves you in an odd place in your file system where you might not be able to get to the notebooks you want to work with.
Also, it can be tedious to activate the virtual environment every time you want to install new packages or launch other programs you might have installed through `pip`.
This will offer some alternatives to manually activating these every time.

## Virtual Environment Shell

### Desktop Shortcut

Right click on your desktop, and go to New -> Shortcut.  In the box that appears, type `cmd \k path\to\activate script`.
For example, my command is `C:\Windows\System32\cmd.exe /k "C:\Users\nathan\ds-venv\Scripts\activate"`.
Hit the `Next` button, and give your shortcut a name (I called mine `ds-venv`)

By default, this opens the `cmd` terminal (with the virtual environment activated) in the `System32` directory, which isDEFINITELY not somewhere we want to be.
To change this default directory, right click on your new shortcut, go to Properties, and change the `Start in` field to `%userprofile%`

### Windows Terminal

## Jupyter Lab
