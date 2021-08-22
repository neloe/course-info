---
title: Setting Up SSH Keys in Linux/Git Bash 
layout: default
category: software
---

This will walk you through generating an SSH key for your computer and adding it to GitHub.
SSH keys can be used for authentication purposes and setting up secure connections to any POSIX computer running an SSH server.
These steps assume that you are using either Git Bash or a bash-like shell in a POSIX-compliant OS.  
If you are using both WSL and Git Bash, you will want to generate separate keys in both shells or either learn how to set up an ssh-agent or change your home directory in WSL (not recommended until I know what side effects that has).

These instructions come directly from [GitHub](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

## Generating the SSH key

If you have a preexisting SSH key you use for other things, you may skip this step if you so desire.

Open your terminal window (Git Bash, WSL terminal, etc), and issue the following command:
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
but replace your email with _an email address associated with your GitHub account_.
If your computer doesn't support ed25519 (you'll know if the command fails), you'll run a different command: `ssh-keygen -t rsa -b 44096 -C "your_email@example.com"`

You will be asked to enter a file location for the key; the default location is the standard location so accept that.
You can choose whether to use a passphrase for your SSH key; I tend to use one key per device and allow them to be passphraseless (once a user has my device I have bigger problems then my SSH key not having a passphrase). 
Hit enter without typing anything else to use an empty passphrase (no passphrase).

## Uploading Your SSH Key to GitHub

In your terminal window, run the following command (assuming you kept the default file location):

```bash
cat ~/.ssh/id_ed25519.pub
```

You can also open this file in any text editor to make copying easier.

If you needed to run the alternate key generation command, you'll run `cat ~/.ssh/id_rsa.pub`.
Note: It is very important that you choose the .pub file; the other is your private key and should _never be shared with anyone else_.
You should see output to your terminal a line that starts with `ssh-ed25519` or `ssh-rsa`, followed by a string of gibberish, followed by your email address.
Copy this entire string to your clipboard.  The output for the ed25519 algorithm is significantly shorter than it is for RSA.

Navigate your web browser to your [Settings](https://github.com/settings/profile) (these links work if you are already logged in to GitHub) by selecting your profile picture in the top right and selecting "Settings".
In the menu on the left, select SSH and GPG keys (or go straight to the [SSH keys page](https://github.com/settings/keys)).
At the top of the settings page you should see something that looks like:

![New SSH Header]({{ "assets/img/ssh-keygen/new-ssh-github.png" | relative_url }})

Click the "New SSH Key" button in the upper right.
In the next screen give the SSH key a title (I tend to use a description of what the key is from; for example: "Home Desktop WSL"), and in the "Key" box, paste your copied key, then click the Add SSH key button.

You can now use the SSH based URLs for working with GitHub repositories on this computer!

## Optional: Enable SSO

If you have [joined the Northwest Organization]({{ "commons/nw_org" | relative_url }}) and want to be able to clone repositories from that organization, you will need to select the "Enable SSO" button next to the key you just added and log in using your Northwest credentials.

