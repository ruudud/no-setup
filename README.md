# No Setup, Installation setup script for Ubuntu Minimal

![Screenshot](https://raw.github.com/charnley/no-setup/master/screenshots/screenshot_1.png)

## Why?

This is a installation script for
[Ubuntu Minimal >=12.04](https://help.ubuntu.com/community/Installation/MinimalCD)
based around the [window manager i3](http://i3wm.org)

The installation script is an alternative work-environment to
the traditional Unity, Gnome3, LXDE, etc based.
We wanted a minimal, fast and productive work-flow
which we found in the tile-based window manager
[i3 window manager](http://i3wm.org/).

So what we present here is a install script based around
the awesome window manager and a minimal Ubuntu setup, mostly
aimed towards power users.

## Installation Instructions

1) Download 'Ubuntu Minimal CD' from
[https://help.ubuntu.com/community/Installation/MinimalCD](https://help.ubuntu.com/community/Installation/MinimalCD).

To make a bootable USB of this, run this command on an **unmounted** USB stick device:

    sudo dd if=mini.iso bs=4096 of=/dev/sdb
    
(To wipe, you can do `sudo dd if=/dev/zero bs=4096 count=256 of=/dev/sdb`.)

Install it on your computer.

Now you have a nice clean setup. No display, no nothing. Enjoy that for a few
seconds, then go to the next step.

2) Install git

    sudo apt-get install git

3) Download installation script.

    git clone git://github.com/ruudud/no-setup.git


4) Run the installation script 'install' from the folder, and remember to run it as administrator.

    cd no-setup
    sudo ./install


5) Run the configuration script for the user you want to configure.

    ./config


6) Restart and Happy i3'ing

    sudo shutdown -r now




