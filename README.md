[![Version](https://img.shields.io/badge/FakeImageExploiter-1.0-orange.svg?maxAge=259200)]()
[![Stage](https://img.shields.io/badge/Release-Alpha-orange.svg)]()
[![Build](https://img.shields.io/badge/Supported_OS-Linux-orange.svg)]()


## FakeImageExploiter v1.0 - backdoor images.jpg[.exe]
    Version release: v1.0 (Alpha)
    Author: pedro ubuntu [ r00t-3xp10it ]
    CodeName: troia_revisited
    Distros Supported : Linux Ubuntu, Kali, Mint, Parrot OS
    Suspicious-Shell-Activity (SSA) RedTeam develop @2016


## LEGAL DISCLAMER:
    The author does not hold any responsibility for the bad use
    of this tool, remember that attacking targets without prior
    consent is illegal and punished by law.



## DESCRIPTION:
    This module takes one existing image.jpg and one payload.exe (input by user) and
    builds a new payload (evil.jpg.exe) that if executed it will trigger the download
    of the 2 previous files stored into apache2 webserver (image.jpg + payload.exe).
    This module also changes the payload Icon to match the input image.jpg Then uses
    'hides known file extensions' to hidde the .exe extension (final: evil.jpg.exe) ..
 
## EXPLOITATION:
    evil.jpg.exe final binary should be deliver to target using social enginnering
    (apache2) to trick user into pressing the fake_image.jpg.exe (malicious binary).
    When executed the evil.jpg.exe will download and open the image.jpg and the
    payload.exe from our apache2 webserver, and execute the two of them (payload hidden) ..
    Credits: https://null-byte.wonderhowto.com/how-to/hide-virus-inside-fake-picture-0168183


## DEPENDENCIES
    xterm, wine, ruby, ResourceHacker(wine)

    'backdoorppt script will work on wine 32 or 64 bits'
    'it also installs ResourceHacker under .../.wine/Program Files/.. directorys'


## DOWNLOAD/INSTALL
    1º - Download framework from github
         wget http ----


    2º - Set files execution permitions
         cd FakeImageExploiter
         sudo chmod +x *.sh


    3º - Run main tool
         sudo ./FIE.sh


## Framework Banner
![venom shellcode v1.0.13](http://4.1m.yt/zNRgR8N.png)
