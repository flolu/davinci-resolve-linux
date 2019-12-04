# Davinci Resolve on Linux (Debian)

<!-- TODO Insert thumbnail as image -->
<!-- TODO Link YouTube video -->

> Davinci Resolve is one of the most powerful **free** video editing software out there. But installing and using the software on Linux can be quite painful at first. This guide will help you to get started with Davinci Resolve on Linux (Ubuntu) in no time.

## Table of Contents

1. Prerequisites
2. Installation
3. Media Import
4. Media Export
5. Uninstall Resolve
6. Handle Common Issues

## 1. Prerequisites

- Debian-bases Linux distribution
- Relatively modern hardware
- NVIDIA graphics card
- NVIDIA graphics driver
  - Determine recommended driver by running
    ```
    ubuntu-drivers devices | grep recommended
    ```
    - The output will look like this:
      ```
      driver   : nvidia-driver-440 - third-party free recommended
      ```
    - Install recommended driver by running:
      ```
      sudo apt install nvidia-driver-440
      ```
    - Reboot
  - Or use this [excellent guide](https://askubuntu.com/questions/61396/how-do-i-install-the-nvidia-drivers/61433#61433)

## 2. Installation

1. Head to https://www.blackmagicdesign.com/products/davinciresolve
2. Click on "Download"
3. Select the free Linux version
4. Unzip `DaVinci_Resolve_XX.Y.Z_Linux.zip` archive
5. Double click `DaVinci_Resolve_XX.Y.Z_Linux.run` and follow installation guide

   - or run `./DaVinci_Resolve_XX.Y.Z_Linux.run`

6. Start Resolve by searching for it in your applications
   - or run `/opt/resolve/bin/resolve`

## 3. Media Import

## 4. Media Export

## 5. Uninstall Resolve

## 6. Handle Common Issues
