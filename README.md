# ds1963s-utils
Utilities and tools for the DS1963S iButton dongle.

## ds1963s-emulator

Emulates work with i-Wire

## ds1963s-tool

Tools for ds1963s for extracting data pages, counters. For ```-f``` option please refer to the ```paper.pdf``` and
```update.pdf``` in the root of the project.

## How to build

    clone repo
    cd src
    cmake .
  
## ds1963s-tool command line options

    Usage: ./ds1963s-tool [OPTION] [DATA]
    Modifiers can be used for several commands.
       -a --address=address  the memory address used in several functions.
       -p --page=pagenum     the page number used in several functions.
       -d --device=pathname  the serial device used.
    
    Function that will be performed.
       -i --info             print ibutton information.
       -f --info-full        print full ibutton information.
       -r --read=size        read 'size' bytes of data.
       -t --read-auth=size   read 'size' bytes of authenticated data.
       -s --sign-data=size   sign 'size' bytes of data.
       -w --write            write data.
       --write-secret=num    write data to secret 'num'.
