#  GDPVALUED

GDPVALUED wallet/daemon management utilities - version 0.1.28 for use of GDPVALUE.

* This script installs, updates, and manages single-user dash daemons and wallets
* It is currently only compatible with 32/64 bit linux.
* Multi-user (system directory) installs are not supported

# Install/Usage

To install gdpvalued do:

    sudo apt-get install python git unzip pv
    cd ~ && git clone https://github.com/gdpvalue/gdpvalued

To update your existing version 12 32/64bit linux dash wallet to the latest
dashd, do:

    gdpvalued/gdpvalued update

To perform a new install of gdpvalued, do:

    gdpvalued/gdpvalued install

To overwrite an existing dash install, do:

    gdpvalued/gdpvalued reinstall

To update gdpvalued to the latest version, do:

    gdpvalued/gdpvalued sync

To restart (or start) gdpvaluedd, do:

    gdpvalued/gdpvalued restart

To get the current status of gdpvaluedd, do:

    gdpvalued/gdpvalued status


# Commands

## sync

"gdpvalued sync" updates gdpvalued to the latest version from github

## install

"gdpvalued install" downloads and initializes a fresh gdpvalued install into ~/.gdpvalued
unless already present

## reinstall

"gdpvalued reinstall" downloads and overwrites existing gdpvalued executables, even if
already present

## update

where it all began, "gdpvalued update" searches for your gdpvaluedd/gdpvalue-cli
executibles in the current directory, ~/.gdpvalued, and $PATH.  It will prompt
to install in the first directory found containing bothgdpvaluedd and gdpvalued-cli.
Multiple wallet directories are not supported. The script assumes the host runs
a single instance of gdpvaluedd.

## restart

"gdpvalued restart [now]" restarts (or starts) gdpvaluedd. Searches for gdpvalued-cli/gdpvaluedd
the current directory, ~/.gdpvalued, and $PATH. It will prompt to restart if not
given the optional 'now' argument.

<a href="#restart-1">screencap</a>

## status

"gdpvalued status" interrogates the locally running gdpvaluedd and displays its status

<a href="#status-1">screencap</a>

# Dependencies

* bash version 4
* nc (netcat)
* curl
* perl
* pv
* python
* unzip
* gdpvaluedd, gdpvalued-cli - version 12 or greater to update

# Screencaps

### install

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalued_0.1-install.png">

### update

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalued_0.1-update.png">

### reinstall

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalued_0.1-reinstall.png">

### restart

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalued_0.1-restart.png">

### status

<img src="https://raw.githubusercontent.com/gdpvalue/gdpvalued/master/screencaps/gdpvalued_0.1-status.png">

# Contact

Click at [GDPVALUE](https://gitter.im/GDPValued/community/) or make a [pull request](Https://github.com/gdpvalue/gdpvalued/).

