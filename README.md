# DaVinci Resolve on Linux (Debian)

<!-- TODO Insert thumbnail as image -->
<!-- TODO Link YouTube video -->

> Davinci Resolve is one of the most powerful **free** video editing software out there. But installing and using the software on Linux can be quite painful at first. This guide will help you to get started with Davinci Resolve on Linux (Ubuntu) in no time.

## Contents

- [Prerequisites](https://github.com/flolude/davinci-resolve-linux#prerequisites)
- [Installation](https://github.com/flolude/davinci-resolve-linux#installation)
- [Media Import](https://github.com/flolude/davinci-resolve-linux#media-import)
- [Media Export](https://github.com/flolude/davinci-resolve-linux#uninstall-resolve)
- [Uninstall Resolve](https://github.com/flolude/davinci-resolve-linux#uninstall-resolve)
- [Handle Common Issues](https://github.com/flolude/davinci-resolve-linux#handle-common-issues)
- [Install NVIDIA driver](https://github.com/flolude/davinci-resolve-linux#install-nvidia-driver)

## Prerequisites

- Debian-bases Linux distribution
- Relatively modern hardware
- NVIDIA graphics card
- [NVIDIA driver](https://github.com/flolude/davinci-resolve-linux#7-install-nvidia-driver)

## Installation

**Method 1** (recommended)

1. Head to https://www.blackmagicdesign.com/products/davinciresolve
2. Click on "Download"
3. Select the free Linux version
4. Unzip `DaVinci_Resolve_XX.Y.Z_Linux.zip` archive
5. Double click `DaVinci_Resolve_XX.Y.Z_Linux.run` and follow installation guide

   - or run `./DaVinci_Resolve_XX.Y.Z_Linux.run`

6. Start Resolve by searching for it in your applications
   - or run `/opt/resolve/bin/resolve`

**Method 2**

1. Head to https://www.blackmagicdesign.com/products/davinciresolve
2. Click on "Download"
3. Select the free Linux version
4. Unzip `DaVinci_Resolve_XX.Y.Z_Linux.zip` archive
5. Head to https://www.danieltufvesson.com/makeresolvedeb
6. Download script with same version as your downloaded Resolve
7. Unzip `makeresolvedeb_XX.Y.Z-X.sh.tar.gz`

- Your folder should now include the following files:
  ```
  DaVinci_Resolve_Studio_XX.Y.Z_Linux.run
  Linux_Installation_Instructions.pdf
  makeresolvedeb_XX.Y.Z-X.sh
  ```

8. Run the `makeresolvedeb` script

- For free version of DaVinci Resolve run:

  ```
  ./makeresolvedeb_XX.Y.Z-X.sh lite
  ```

- For Studio version of DaVinci Resolve run:

  ```
  ./makeresolvedeb_XX.Y.Z-X.sh studio
  ```

9. Install the Resolve via the created `.deb` file

- Double click and click "Install"
- Or run in terminal:

  ```
  sudo dpkg -i davinci-resolve_XX.Y.Z-X_amd64.deb
  ```

10. If you get an error saying "Sorry. Need 'xyz' to continue", just install it

- For example if the error is: "Sorry. Need 'xorriso' to continue", you should run:

```
sudo apt-get install xorriso
```

## Media Import

## Media Export

## Uninstall Resolve

**Method 1** (recommended)

Run the same script, you used for installing Resolve (`DaVinci_Resolve_XX.Y.Z_Linux.run`) and choose "Uninstall DaVinci Resolve" in the second step.

**Method 2**

```
sudo rm -f -r /opt/resolve
sudo rm -f -r ~/Documents/BlackmagicDesign
```

## Handle Common Issues

## Install NVIDIA driver

Determine recommended driver by running

```
ubuntu-drivers devices | grep recommended
```

The output will look like this:

```
driver : nvidia-driver-440 - third-party free recommended
```

Install recommended driver by running:

```
sudo apt install nvidia-driver-440
```

Then reboot you computer.

---

> Alternatively you can use this [excellent guide](https://askubuntu.com/questions/61396/how-do-i-install-the-nvidia-drivers/61433#61433)
