---
title: "Setting up the Development Environment"
layout: page
permalink: /pages/tutorials/setup/setup-dev-env.html

tags: [software]
keywords: software
sidebar: home_sidebar
toc: false
---



## 1. Install Dependencies

### 1.1 VirtualBox
VirtualBox is used to run the virtual machine used as the development environment. Get it [here](https://www.virtualbox.org/wiki/Downloads).


### 1.2 Install Vagrant

Vagrant is used to set up the virtual machine used as the development environment. Get it [here](https://www.vagrantup.com/downloads).

### 1.3 Install the Guest Additions Plugin

The Vagrant guest additions plugin automatically installs VirtualBox guest additions into the virtual machine. Install it
by opening up a command prompt (Windows) or a terminal (Linux/Mac) and running the following:

```
vagrant plugin install vagrant-vbguest
```

## 2. Set up the Vagrant Box


Download the development environment tools from here



### 2.1 Download the Artemis Box

Download the Vagrant box [here]() to a place you want to run Vagrant from.

### 2.2 Add the Artemis Box

From a command prompt or terminal window, enter the following (using the path you downloaded the Vagrant box to):

```
cd PATH/TO/VAGRANT/BOX
vagrant box add artemis.box
```

### 2.3 Create the Machine

Next, enter the following (using the path you want to run the box from):

```
cd PATH/TO/VM
vagrant init
vagrant up
```

After a minute or so you should see the virtual machine boot.

## 3. Update Software

{% include tip.html content="This step is optional. Follow this step if you want to make sure you have the
latest software." %}

From the virtual machine, open a new terminal (<kbd>Control</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd>) and run the following commands:


```bash
$ cd
$ git clone https://github.com/mtmk-ee/artemis-cubesat-kit.git
$ cd artemis-cubesat-kit
$ sudo chmod +x update
$ ./update
```

You will be prompted whether or not you want to update various components. Entering `y` will overwrite the existing
installations.

