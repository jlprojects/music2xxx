# music2xxx
## Hybrid Music 2000 Clone Midi I/O PCB

This is a hardware clone of the Hybrid Music 2000 Midi add-on for the Acorn BBC Microcomputer model B and Master 128 designed for use with the Hybrid Music 5000 system. It is designed to stack on the Music5xxx clone PCB, and uses the 5V supply from the main board. If used independently of the Music5xxx, you will need to provide a 5V supply - this can come from the BBC Micro's auxiliary power connector.

The Music 2000 Midi interface combined with the AMPLE programming language and the Hybrid Studio 5000 Studio software provides versatile control of external Midi devices. The Music 2000 has 3 Midi output sockets.

Despite having an on-board Midi input port, AMPLE and the Hybrid System cannot use it directly. It is assumed that the Hybrid system is used as a controller and sequencer. However, it is possible to address the interface from user programs.

## The clone
![music5xxx PCB render](https://github.com/jasonl-beeb/music2xxx/raw/master/images/music2xxx-render.png)

It is designed in Kicad, based upon Colin Fraser's reverse-engineered schematic. http://www.colinfraser.com/m5000/m2000sch.pdf This version uses a different opto-isolator on the Midi input, and implements activity LEDs for the Midi outputs. 

Currently all the 74xx series logic ICs are available new. The 6850 UART ICs are no longer manufactured, but are commonly available second-hand or new-old-stock. 

4/9/19 For standalone use, an optional LM7805 regulator is added to allow powering the board from 9V-12V, as well as an LED to show input activity. A few prototype PCBs have been ordered.

## Using outside the Hybrid system

It's possible to use the m2000 Midi interface in BASIC or machine code - the 6850 Uarts can be read to or written to at addresses: 

* FC08/9 ACIA 1 (MIDI OUT 1)
* FC0A/B ACIA 2 (MIDI OUT 2)
* FC0C/D ACIA 3 (MIDI OUT 3, MIDI IN)

Info from: http://mdfs.net/Info/Comp/BBC/MIDI/m2000

## Resources

* Colin Fraser's Music5000 Resources: http://www.colinfraser.com/m5000/m5000.htm

* The Music2000 Interface User Guide covers all aspects of controlling Midi instruments with AMPLE and Studio 5000. It's available on the retro-kit archive page describing the Hybrid Music 2000: https://www.retro-kit.co.uk/page.cfm/content/Hybrid-Music-2000-Interface/

* A comprehensive archive about the Hybrid Music System: https://www.retro-kit.co.uk/page.cfm/content/Hybrid-Music-5000-Synthesiser/

* Here's the Stardot thread about this project: https://stardot.org.uk/forums/viewtopic.php?f=3&t=16895

* The Stardot 8bit hardware forum often has posts about the Hybrid Music system: https://stardot.org.uk/forums/viewforum.php?f=3

* Information about Midi on the BBC Microcomputer: http://mdfs.net/Info/Comp/BBC/MIDI/

## Licence

Unless otherwise marked, work in this repository is licenced under [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/)  ![Creative Commons Licence](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)
