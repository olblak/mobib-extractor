# About

MOBIB-extractor allows you to read the data stored on your STIB Mobib card.

# Screenshot

Everybody loves screenshots :-)

![MOBIB Extractor screenshot](https://raw.githubusercontent.com/zoobab/mobib-extractor/master/mobib-extractor-screenshot.png)

# License

(c) 2009 MOBIB Extractor project. This software is provided 'as-is',
without any express or implied warranty. In no event will the authors be held
liable for any damages arising from the use of this software.

Permission is granted to anyone to use this software for any purpose,
including commercial applications, and to alter it and redistribute it
freely, subject to no restriction.

Technical remarks and questions can be addressed to
<tania.martin@uclouvain.be>
<jean-pierre.Szikora@uclouvain.be>

# Installation

## on Linux

You must install:
- pcsc_lite
- ccid
- python
- the python library PIL 
- pyscard

If you use the smartcard reader ACS ACR38, you have to install the
corresponding package.


## on Mac OS X 10.5.6 (last version)

As this new version contains pcsc_lite, ccid and python, you only have to
install:
- the python library PIL
- pyscard (the mpkg is easily found on the web)
If you use the smartcard reader ACS ACR38, the driver mpkg can be found on the
manufacturer (ACS) website.


## on Windows

You must install:
- python
- the python library PIL
- pyscard
If you use the smartcard reader ACS ACR38, the driver can be found on the
manufacturer (ACS) website.

# Run

You can then launch the application MOBIB-Extractor.py in the terminal using
the command:
- For UNIX architecture : ./MOBIB-Extractor.py or python MOBIB-Extractor.py
- For Windows : MOBIB-Extractor.py

# User manual

1. If you want to read a card:
  * Plug your reader and put your card on
  * Click File and click Acquisition
2. If you want to read an old dump file card:
  * Click File and click Open dump
  * Then select the file you want to read
3. If you want to save a dump card:
  * Click File and click Save dump
  * Then choose the name and directory to record the dump

# Keyboard shortcuts

- ```<Double-Click>``` to zoom + or -
- ```<MouseWheel>``` to vertical scroll
- ```<Left arrow>``` to scroll left
- ```<Right arrow>``` to scroll right
- ```<Up arrow>``` to scroll up
- ```<Down arrow>``` to scroll down
- ```<Esc>``` to leave the program
- ```<a>``` to dump a card
- ```<o>``` to open a dump
- ```<s>``` to save a dump

# Working USB readers

* Advanced Card Systems (ACR) ACR122: Bus 002 Device 002: ID 072f:2200 Advanced Card Systems, Ltd ACR122U

# Todo

* add a requirements.txt
* add a list of tested and working readers
* dump the content with an NFC reader with Nexus5 and read it?
* add a docker container
* CLI output next to this TK graphical interface
* TK interface is too big

# Links

* https://github.com/QKaiser/mobib-extractor : CLI version working! Screenshot:
```
$ ./extract.py
Smartcard reader detected.
Connecting to ACS ACR122U PICC Interface 00 00...
 
Card number: 6396532009560098406
Name: Mr BENJAMIN BERNARD HENRION                          
Birthday: 11 / 09 / 1979
Zip code: 0
Contract type: UNKNOWN
Remaining travels: 0
 
Last known locations:
 
Transport   Line    Station     Time
Metro       1A/1B   Maelbeek        16/09/2017 11:47
Metro       1A/1B   Sainte Catherine        08/09/2017 18:53
-       0   No info     - 0:00
```
