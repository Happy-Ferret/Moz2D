# Moz2D [![Build Status](https://travis-ci.org/syrel/Moz2D.svg?branch=master)](https://travis-ci.org/syrel/Moz2D) [![Build status](https://ci.appveyor.com/api/projects/status/b3bjd40ckj4e8n52/branch/master?svg=true)](https://ci.appveyor.com/project/syrel/moz2d/branch/master) [ ![Download](https://api.bintray.com/packages/syrel/Moz2D/libMoz2D/images/download.svg) ](https://bintray.com/syrel/Moz2D/libMoz2D/_latestVersion) [![Coverage Status](https://coveralls.io/repos/github/syrel/Sparta/badge.svg?branch=master)](https://coveralls.io/github/syrel/Sparta?branch=master)
Scripts to compile `gfx` part of Mozilla Firefox as single shared library


Compile shared library (32 bit):

`./build.sh --arch i386`

Or 64 bit:

`./build.sh --arch x86_64`

Binary will be in `build/` folder

## Dependencies
Tools:<br>
`git >= 1.7.12` `node >= v0.11.12` `python` `cmake >= 3.0` `make` `autoconf 2.13` `gcc-multilib >= 5.3`<br>
Utilities:<br>
`wget` `patch` `which` `tar`

### Ubuntu / Travis

General dependencies:

	sudo apt-get install git nodejs cmake autoconf2.13 yasm


#### 64bit

The following packages are required to build 64bit plugin

	sudo apt-get install libgtk2.0-dev libgtk-3-dev libgconf2-dev
	sudo apt-get install libasound2-dev libpulse-dev
	sudo apt-get libxt-dev libxext-dev libxcb-shm0-dev libx11-xcb-dev

#### 32bit

Make sure to register i386 architecture

	sudo dpkg --add-architecture i386
	sudo apt-get update
	export PKG_CONFIG_PATH=/usr/lib/i386-linux-gnu/pkgconfig/

32bit build requires a few additional packages

	sudo apt-get install gcc-multilib g++-multilib
	sudo apt-get install libglib2.0-dev:i386 libatk1.0-dev:i386 libcairo2-dev:i386 libgdk-pixbuf2.0-dev:i386 libpango1.0-dev:i386 libgtk2.0-dev:i386

	sudo apt-get install libxkbcommon-dev:i386 libgtk-3-dev:i386
	sudo apt-get install libfreetype6-dev:i386 libgconf2-dev:i386
	sudo apt-get install libasound2-dev:i386 libpulse-dev:i386
	sudo apt-get install libxt-dev:i386 libxext-dev:i386 libxcb-shm0-dev:i386 libx11-xcb-dev:i386

### Windows (in progress)
