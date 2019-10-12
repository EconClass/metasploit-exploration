# [Exploring Exploits](https://econclass.github.io/metasploit-exploration/)

The purpose of this document is to familiarize new developers, such as myself, with some of the exploits detailed in the Metasploit penetration testing platform. Through this exploration, the hope is to gain insight into some of the attack vectors that are taken into account in the software industry. Ultimately, I hope to make the process of exploring web security as beginner friendly as possible. However, I do acknowledge that there are certain aspects of security that are inevitably heavy on technical details.

## The Tools

Before we get to the technologies the remainder of the document will assume that you are familiar with the concept of Virtual Machines.
[Here](https://www.howtogeek.com/196060/beginner-geek-how-to-create-and-use-virtual-machines/) is a great article that goes over the concept and features of Virtual Machines.
That said this walkthrough will be using the following technologies:

| Tool | Description|
|---|---|
| [Metasploit](metasploit.help.rapid7.com/docs/getting-started) | This lets us find, exploit, and validate vulnerabilities from our Command Line |
| [Metasploitable](github.com/rapid7/metasploitable3/) | This is an intentionally vulnerable Virtual Machine for us to test out exploits on |
| [VirtualBox](virtualbox.org) | This is what we will be using to host our metasploitable environment from our own computer |

**NOTE:* The Metasploitable Virtual Machine requires that you install [Packer](www.packer.io/intro/getting-started/install.html) and [Vagrant](https://www.vagrantup.com/docs/installation/) to install and build the Metasploitable.
I recommend installing these dependencies through your Operating System's designated package manager such as `brew` for OSx or `apt` for Ubuntu based Linux distributions.
