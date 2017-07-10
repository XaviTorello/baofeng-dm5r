# Baofeng DM-5R

Links, info and utilities for the Baofeng DM-5R two-way DMR radio.

So far, do not exist any tool to program this talkie over GNU/Linux or MacOS, so the unique way is to do this over a Windows environment (can be virtualized).

This repo contains info and resources fetched from different sources, the main [Baofeng site](https://baofengtech.com/), [Radioddity](radioddity.com)


## Links

* [Manual](https://github.com/XaviTorello/baofeng-dm5r/raw/master/files/DM-5R_User_Maunal.pdf)
  * [Alternative link](http://s3.image.ro.s3.amazonaws.com/download/DM-5R%20User%20Maunal.pdf)
* [Programming software](https://github.com/XaviTorello/baofeng-dm5r/raw/master/files/DM-5R_Programming_Software.rar)
  * Password `123456` (_setted by Raddiodity.com_)
  * [Alternative link](http://s3.image.ro.s3.amazonaws.com/download/DM-5R%20Programming%20Software.rar)
* [Win drivers](https://github.com/XaviTorello/baofeng-dm5r/raw/master/files/Win_Driver_Prolific_3_2_0_0.exe)
  * [Alternative link](http://www.miklor.com/COM/UV_Drivers.php)

---------


## Installation

### Drivers

Take care about to install the [Win drivers](https://github.com/XaviTorello/baofeng-dm5r/raw/master/files/Win_Driver_Prolific_3_2_0_0.exe) **after plug the USB programming cable**.

If not, a manual downgrade of the drivers must be performed in order to make it works.

The latest available _Prolific drivers_ brakes the communication with the DM-5R, so ensure to select the version 3.2.0.0 from the related section.

The install process is very easy, open the EXE, and just follow the assistant. A reboot is not needed.

### Programming software

Decompress the RAR file (password `123456`), and execute the installer. Follow the assistant and start the utility

---------

## Programming the radio

First connect the USB to serial cable to the radio, and to your PC. Be sure to connect it properly, and start the radio.

Take care to select a channel without any kind of activity.

Start the Programming utility, and enforce the connection with the radio.

By default the _Prolific driver_ assigns the radio to the COM3 port; select `COM3` port and keep the default connection speed.

Once the connection is performed, dump the current config reading from the radio.

A visual editor will be showed with all the available configurations.

**Save current config** as a backup after changing anything, ensure that a rollback can be easily performed!

Change whatever you want, and write changes to the radio to save it.
