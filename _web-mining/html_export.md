---
title: Exporting Python Notebooks to HTML 
category: software
layout: default
---

There is the possibility that exporting your notebook fails with the error "tuple is not callable" (or something similar). 
Here are some options that we identified in class to work around this odd software regression.

## Option 1: Run `jupyter notebook`

Instead of starting JupyterLab, from your virtual environment run the command `jupyter notebook`.  
From there, you can navigate to your notebook, open it, and Export it as an HTML file from the File menu

## Option 2: Open `lab` from `notebook`

Start `jupyter notebook` from your virtual environment, then modify the url: replace `tree` with `lab`.
Some people had mixed luck with this working and letting them get to the Lab UI (required a workspace clearing and a refresh)

## Option 3: Command Line `nbconvert`

It is possible to manually run the `nbconvert` command from the command line.
From a console where your virtual environment is activated, run the following command:
```bash
jupyter nbconvert --to=html PATH_TO_NOTEBOOK
```

For example:

![Example nbconvert run]({{ "assets/img/python_venv/nbconvert.png" | relative_url }})
