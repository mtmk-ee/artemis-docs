---
title: Development Environment
permalink: /pages/documentation/other/development-environment.html
layout: page

keywords: software
---

## Introduction

The development environment collectively refers to an [Ubuntu 18.04.3](https://en.wikipedia.org/wiki/Ubuntu_version_history#Ubuntu_18.04_LTS_(Bionic_Beaver)) disk image, and the tools and flight software it contains. Most of the setup and installation is already taken care of in this image.

## What's Inside

* Flight Software
  * BeagleBone Software
    * Agent source code (located under `~/cosmos/source/projects/cubesat-kit`)
    * Pre-compiled agents (located under `~/cosmos/source/projects/cubesat-kit/build`)
  * Raspberry Pi Software
    * Artemis Python Library (located under `~/artemisraspberrypi/artemis`)
    * Example camera script (located at `~/raspberrypi/camera.py`)
  * PyCubed Software
    * Main code (located under `~/pycubed`)
* COSMOS
  * COSMOS (dev branch)
    * SimpleAgent template project (located under `~/cosmos/source/projects/simpleagent_template`)
  * COSMOS Web
* Other
  * Qt Creator
    * ARM Cross Compiler
  * Scripts for convenience
    * Copy built agents to the BeagleBone (`~/copy_agents`)
    * Start COSMOS Web (`~/cosmos-web`)
  * MongoDB Server
  * Doxygen
  * CMake


## Download from GitHub

As updates are released, you'll be able to find new images hosted on our GitHub repository.




## Built-In Scripts

### Update Script

This script updates the local copy of the cubesat kit repository. If you want to update your software, use this script.

Location: home directory
Usage:

```bash
$ ./update
```
