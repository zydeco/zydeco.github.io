---
layout: page
title: Mini vMac for iOS
short_title: Mini vMac
section: ios
permalink: iphone/minivmac
---

This is my port of the [Mini vMac](http://www.gryphel.com/c/minivmac/) emulator
to iOS 9. You can see it in action on this video:

{% include youtube.html id="w9U42hqhdzA" width="720" %}

## Features

* Emulates 4MB Mac Plus
* Full simulated keyboard (including all Mac keys)
* Full sound output
* Uses external keyboard if available
* Regulable emulation speed (up to 8x)
* Easy(ish) to import/export disk images

## Requirements

* iOS 9 or later
* Mac Plus ROM image
* Disk images with Mac software
* A Mac with Xcode 7 (required to build)

## Download

* {% include link-icon.html icon="social-github" url="https://github.com/zydeco/minivmac4ios" name="Source Code on GitHub" %}

## Usage

### ROM and Disk Images

You can import the ROM (`vMac.ROM`) and disk images (with `.dsk` or `.img`
extension) into Mini vMac from other apps (iCloud Storage, Dropbox, etc), using
AirDrop, or via iTunes File Sharing.

![Disk Images](/images/minivmac4ios/disks.png)


* To insert disk images, swipe left with two fingers and the list of disks will
    appear. Icons are automatically generated based on the contents of the disk.
* Tap an hold on a file to delete, rename or share
* Tap the Edit button to show all files, and the Create Disk Image option

![Create New Disk](/images/minivmac4ios/newdisk.png)


The disk image menu will attempt to find an icon from the following sources (in
descending order of priority):

1. Volume icon (System 7)
2. Application icon, if the disk contains only one application
3. Application matching the name of the volume (not the disk image)
4. Application with name written in the comment field of the volume

If no icon is found, it will show a standard floppy disk icon.

### Keyboard

Swipe up with two fingers to show the keyboard, and down to hide it.

![Keyboard](/images/minivmac4ios/keyboard.png)

The emulated keyboard features all the keys on an Apple Extended keyboard
(except the Power key). The Command, Option , Control and Shift keys are
sticky, to make keyboard shortcuts easier to type. You can change the
appearance of the emulated keyboard in the settings.

If you have an external keyboard attached, you can use it too, although some
shortcuts may interfere with iOS.

### Mouse

You can choose to use the screen as a touchscreen, where tapping on the screen
acts a mouse click, or as a trackpad. In trackpad mode, dragging is done by
tapping twice fast and holding it down.

### Settings

![Settings](/images/minivmac4ios/settings.png)

Swipe right with two fingers to show the settings dialog, where you can change
the following:

* **Speed:** make the emulated machine faster than a Mac Plus
* **Mouse Type:** switch between touchscreen and trackpad mode
* **Keyboard Layout:** change the layout of the emulated keyboard

### Credits

* Mini vMac for iOS by [Jesús A. Álvarez](https://github.com/zydeco)
* [Mini vMac](http://gryphel.com/c/minivmac/) ©2001-2016 Paul C. Pratt
* [vMac](http://vmac.org/) ©1996-1999 Philip Cummins & al.
* [hfsutils](http://www.mars.org/home/rob/proj/hfs/) ©1996-2000 Robert Leslie

## Version History

#### 2.0 - 23<sup>rd</sup> May 2016

* Updated Mini vMac core to 3.4 alpha
* Universal UI for iPhone and iPad
* Doesn't require jailbreak
* More complete emulated keyboard
* Regulable emulation speed
* Supports external keyboard
* Import/export disk image files from/to other apps

#### 1.x - 2008-2011

* See [this page](/minivmac4iphone)