# Roland UA-100 Mixer
### An incomplete PyQT5 Mixer/DSP Controller for the Roland UA-100 Audio Interface

Authors: https://github.com/wishmerhill, https://github.com/wrongontheinternet, https://github.com/mo-g

Wishmerhill wrote this in QT4, WrongOnTheInternet rewrote it for QT5, and mo-g fixed some deprecated statements so it would run on Ubuntu Studio 26.04. And also renamed it and updated the documentation a bit. Also there was no licence file and the code only had a variable pointing to an unversioned "GPL". So I'm making the gross assumption that it's intended to be GPLv3.0 (as that was current when this was written) and have added the licence file and header accordingly.

Also, for easy future versioning, I dub this Version 0.7.0 - with 0.5.x as the last release by wishmerhill, 0.6.x as the rewrite by wrongontheinternet and 0.7.x as the patched version by mo-g.

## Installation and Use

### Prerequisites

This is ONLY tested on Ubuntu Studio 26.04 LTS. It seems perfectly happy interacting through Pipewire, so there's no need to do anything to your audio configuration. Feel free to submit patches to fix it for other distro's (including just adding prerequisite options) but anything that breaks Resolute Racoon will be rejected until April 2031.

apt install python3-numpy python3-rtmidi python3-mido python3-sounddevice

### Install

To install Roland UA-100 Mixer just clone the git repo to your computer. 

#### With git

```shell
$ mkdir ~/Applications
$ git clone https://github.com/mo-g/Roland-UA100-Mixer.git ~/Applications/Roland-UA100-Mixer
```
#### Without git

If you don't have git and don't want to install one you can just open https://github.com/mo-g/Roland-UA100-Mixer and click "Clone or download"-> "Download ZIP" in top-right corner of the page, then extract files wherever you like.

### Run Roland UA100 Mixer

From the ua100mix directory, launch main.py with your python interpreter:

```shell
$ cd ~/Applications/Roland-UA100-Mixer
$ python main.py
```

A sample .desktop file is included. Download a Roland logo, update the .desktop file to replace 'user' with your username, and copy it to ~/.local/share/applications/ for it to appear in the Audio Production/Mixers and Card Control menu, just as it should.


###### A word about the "SaxMode" icon
I use this mixer mainly to record my exercises with the saxophone, so I need a quick way to set the input and output levels as well as the recording and playback sources.

![Just a sample screenshot...](/screenshots/ua-100_mix.png?raw=true "UA-100 Mixer at work")

Tags: Roland, Edirol, UA-100, UA 100, mixer, effects, python, pyqt, ubuntu studio, 26.04, resolute raccoon
