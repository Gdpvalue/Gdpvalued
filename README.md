#  GDPVALUE

GDPVALUE wallet/daemon management utilities - version 0.1.28 for use.

* This script installs, updates, and manages single-user gdpvalue daemons and wallets
* It is currently only compatible with 32/64 bit linux.
* Multi-user (system directory) installs are not supported

# Install/Usage

To install gdpvalue do:

    sudo apt-get install python git unzip pv
    cd ~ && git clone https://github.com/gdpvalue/gdpvalued

To update your existing version 12 32/64bit linux gdpvalue wallet to the latest
dashd, do:

    gdpvalue/gdpvalue update

To perform a new install of gdpvalued, do:

    gdpvalue/gdpvalue install

To overwrite an existing gdpvalue install, do:

    gdpvalue/gdpvalue reinstall

To update gdpvalue to the latest version, do:

    gdpvalue/gdpvalue sync

To restart (or start) gdpvalued, do:

    gdpvalue/gdpvalue restart

To get the current status of gdpvalue, do:

    gdpvalue/gdpvalue status


# Commands

## sync

"gdpvalue sync" updates gdpvalue to the latest version from github

## install

"gdpvalue install" downloads and initializes a fresh gdpvalue install into ~/.gdpvalue
unless already present

## reinstall

"gdpvalue reinstall" downloads and overwrites existing gdpvalue executables, even if
already present

## update

where it all began, "gdpvalue update" searches for your gdpvalued/gdpvalue-cli
executibles in the current directory, ~/.gdpvalue, and $PATH.  It will prompt
to install in the first directory found containing bothgdpvalued and gdpvalue-cli.
Multiple wallet directories are not supported. The script assumes the host runs
a single instance of gdpvalued.

## restart

"gdpvalue restart [now]" restarts (or starts) gdpvalued. Searches for gdpvalue-cli/gdpvalued
the current directory, ~/.gdpvalue, and $PATH. It will prompt to restart if not
given the optional 'now' argument.

<a href="#restart-1">screencap</a>

## status

"gdpvalue status" interrogates the locally running gdpvalued and displays its status

<a href="#status-1">screencap</a>

# Dependencies

* bash version 4
* nc (netcat)
* curl
* perl
* pv
* python
* unzip
* gdpvalued, gdpvalue-cli - version 12 or greater to update

# Screencaps

### install

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalue_0.1-install.png">

### update

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalue_0.1-update.png">

### reinstall

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalue_0.1-reinstall.png">

### restart

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalue_0.1-restart.png">

### status

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalue_0.1-status.png">

# Contact

Click at [GDPVALUE](https://gitter.im/GDPValued/community/) or make a [pull request](Https://github.com/gdpvalue/gdpvalued/).

