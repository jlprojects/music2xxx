# music2xxx
## Hybrid Music 2000 Clone Midi I/O PCB

This is a hardware clone of the Hybrid Music 2000 Midi add-on for the Acorn BBC Microcomputer model B and Master 128 designed for use with the Hybrid Music 5000 system. It is designed to stack on the Music5xxx clone PCB, and uses the 5V supply from the main board. If used independently of the Music5xxx, you will need to provide a 5V supply - this can come from the BBC Micro's auxiliary power connector.

The Music 2000 Midi interface combined with the AMPLE programming language and the Hybrid Studio 5000 Studio software provides versatile control of external Midi devices. The Music 2000 has 3 Midi output sockets.

Despite having an on-board Midi input port, AMPLE and the Hybrid System cannot use it directly. It is assumed that the Hybrid system is used as a controller and sequencer. However, it is possible to address the interface from user programs.

## The clone

![music5xxx PCB render](https://github.com/jasonl-beeb/music2xxx/raw/master/images/music2xxx-render.png)

It is designed in Kicad, based upon Colin Fraser's reverse-engineered schematic. http://www.colinfraser.com/m5000/m2000sch.pdf This version uses a different opto-isolator on the Midi input, and implements activity LEDs for the Midi outputs. 

Currently all the 74xx series logic ICs are available new. The 6850 UART ICs are no longer manufactured, but are commonly available second-hand or new-old-stock. 

## Resources

* Colin Fraser's Music5000 Resources: http://www.colinfraser.com/m5000/m5000.htm

* The Music2000 Interface User Guide covers all aspects of controlling Midi instruments with AMPLE and Studio 5000. It's available on the retro-kit archive page describing the Hybrid Music 2000: https://www.retro-kit.co.uk/page.cfm/content/Hybrid-Music-2000-Interface/

* A comprehensive archive about the Hybrid Music System: https://www.retro-kit.co.uk/page.cfm/content/Hybrid-Music-5000-Synthesiser/

* Here's the Stardot thread about this project: https://stardot.org.uk/forums/viewtopic.php?f=3&t=16895

* The Stardot 8bit hardware forum often has posts about the Hybrid Music system: https://stardot.org.uk/forums/viewforum.php?f=3

## Licence

Unless otherwise marked, work in this repository is licenced under [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/)  ![Creative Commons Licence](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)
