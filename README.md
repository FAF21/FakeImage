[![Version](https://img.shields.io/badge/FakeImageExploiter-1.1-orange.svg?maxAge=259200)]()
[![Stage](https://img.shields.io/badge/Release-Alpha-orange.svg)]()
[![Build](https://img.shields.io/badge/Supported_OS-Linux-orange.svg)]()


![FakeImageExploiter v1.1](http://2.1m.yt/EASUSH9.png)


## FakeImageExploiter v1.1 - backdoor images.jpg[.exe]
    Version release: v1.1 (Alpha)
    Author: pedro ubuntu [ r00t-3xp10it ]
    CodeName: troia_revisited
    Distros Supported : Linux Ubuntu, Kali, Mint, Parrot OS
    Suspicious-Shell-Activity (SSA) RedTeam develop @2017



## Legal Disclamer:
    The author does not hold any responsibility for the bad use
    of this tool, remember that attacking targets without prior
    consent is illegal and punished by law.

<br /><br />

## Description:
    This module takes one existing image.jpg and one payload.exe (input by user) and
    builds a new payload (evil.jpg.exe) that if executed it will trigger the download
    of the 2 previous files stored into apache2 webserver (image.jpg + payload.exe).
    This module also changes the payload Icon to match one file.jpg icon. Then uses
    'hide known file extensions' to hidde the .exe extension (final: evil.jpg.exe) ..


 
## Exploitation:
    evil.jpg.exe final binary should be deliver to target using social enginnering
    (apache2) As soon as the victim runs our executable, our picture will be downloaded
    and opened in the default picture viewer, our malicious payload will be executed,
    and we will get a meterpreter session.

    'This tool will upload all files to apache2, and starts payload currespondent handler' 



## Payloads accepted (user input):
    payload.exe | payload.ps1 | payload.txt [Metasploit]



## Pictures accepted (user input):
    All pictures with .jpg (default) | .jpeg | .bmp  extensions (all sizes)
    "Edit 'settings' file before runing tool to sellect another extension"

<br /><br />

## Dependencies:
    xterm, zenity, apache2, mingw32[64], ResourceHacker(wine)
    'Auto-Installs ResourceHacker.exe under ../.wine/Program Files/.. directorys'

    WARNING: The ResourceHacker provided by this tool requires WINE set to windows 7
    WARNING: To change icon manually (resource hacker bypass) edit 'settings' file.



## Download/Install:
    1º - Download framework from github
         git clone https://github.com/r00t-3xp10it/FakeImageExploiter.git

    2º - Set files execution permitions
         cd FakeImageExploiter
         sudo chmod +x *.sh

    3º - Run main tool
         sudo ./FakeImageExploiter.sh

## Framework Banner
![FakeImageExploiter v1.1](http://3.1m.yt/iCIwNdy.png)

