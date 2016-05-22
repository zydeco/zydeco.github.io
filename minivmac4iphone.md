---
layout: page
title: Mini vMac for iPhone
short_title: Mini vMac
section: ios
permalink: iphone/minivmac
---

This is my port of the [Mini vMac](http://www.gryphel.com/c/minivmac/) emulator
to iOS (2.2 to 5.x). This video shows some features of an early version:

{% include youtube.html id="SyS8lOBBk8I" %}

## Features

* 4MB Mac Plus
* Full screen (scaled down) or scrolling (full size)
* Full simulated keyboard (including all Mac keys)
* Sound

## Requirements

* Jailbroken iPhone or iPod Touch
* iPhone OS 2.2 to 5.x
* [Mac Plus ROM image](http://www.gryphel.com/c/minivmac/start.html)
* Disk images with Mac software

## Download

* <a class="icon-social-github" href="https://github.com/zydeco/minivmac4iphone"> Source Code on GitHub</a>

## Usage

### ROM Installation

The ROM file must be named `vMac.ROM` and placed in `/var/mobile/Library/MacOSClassic`

### Disk Images

Disk images should have `.img` or `.dsk` extensions, and be located in
`/var/mobile/Library/MacOSClassic` for them to show up in the disk chooser.

![Disk Chooser](/images/minivmac4iphone/1-insert-disk.png)

* To insert disk images, swipe left with two fingers and the list of disks will
    appear. Icons are automatically generated based on the contents of the disk.

* To delete a disk image, swipe left on it and the delete button will show if disk
    image deletion is enabled (in Settings).

![Create Disk Image](/images/minivmac4iphone/2-new-disk.png)

* To create a new disk image, press the `+` button in the disk image chooser.
    Write a name and use the slider to choose a size between 400KiB and 125MiB.

### Keyboard

Swipe up with two fingers to show the keyboard, and down to hide it.

![Keyboard](/images/minivmac4iphone/3-keyboard.png)

The emulated keyboard features all the keys on the Mac Plus keyboard, except
the keypad. The Command, Option and Shift keys are sticky, to make keyboard
shortcuts easier to type. You can change the keyboard layout and opacity in the
settings.

### Mouse

You can choose to use the screen as a touchscreen, where tapping on the screen
acts a mouse click, or as a trackpad. In trackpad mode, dragging is done by
tapping twice fast and holding it down.

### Screen

You can toggle between full screen (the Mac screen is scaled down to fit the
iPhone) or full size (the Mac screen is shown at its real size) by tapping the
screen with two fingers. In full size mode, you can scroll by tapping the edges.

### Settings

Swipe right with two fingers to show the settings dialog, where you can change
the following:

* **Mouse:** switch between touchscreen and trackpad mode
* **Sound:** enable/disable different sounds from the emulator
* **Disk Images:** enable/disable disk image deletion, and automatic icon creation
* **Keyboard:** change the keyboard layout and opacity

![Settings](/images/minivmac4iphone/4-settings.png)

On the bottom, you can find the [Interrupt and Reset buttons](https://en.wikipedia.org/wiki/Programmer%27s_key).

### Suspend

If you press the home button while the emulated Mac has disks inserted, Mini
vMac will pause but stay open, and show this by displaying the Mac's screen in
its icon. To quit Mini vMac properly, eject all disks before pressing home.
Note that when Mini vMac is suspended, it still uses memory and could be forced
to quit if the memory is low.

![Off and suspended icon](/images/minivmac4iphone/5-suspended-icon.png)

## Version History

#### 1.2.2 - 4<sup>th</sup> May 2011

* Fixed crash on iOS 4.3.x

#### 1.2.1 - 3<sup>rd</sup> October 2009

* Removed SBCustomIcon dependency for iOS 4 compatibility
* Minor interface changes

#### 1.2 - 20<sup>th</sup> June 2009

* iPhone OS 3.0 compatibility
* Handles checksums in Disk Copy 4.2 images
* Hebrew localization and keyboard layout (Gil Osher)
* British keyboard layout
* Minor interface changes

#### 1.1 -  7<sup>th</sup> February 2009

* Create and delete disk images
* Plays sound when disks are ejected
* Trackpad mode
* Application icons in disk list
* Mac screen in icon when suspended

#### 1.0.2 - 27<sup>th</sup> November 2008

* Sound emulation
* Allow uppercase disk extensions
* Close Settings View after Interrupt/Reset
* Finds keyboard layouts in `(~)/Library/MacOSClassic`
* Shows version in Settings View
* Faster and more accurate Video
* Hard Disk Icon
* Fixed Clock emulation
* Fixed keyboard layout changing bug
* Spanish Localization