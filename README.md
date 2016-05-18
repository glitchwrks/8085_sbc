# Glitch Works 8085 SBC

This repository contains the recovered EAGLE projects for the various PC boards designed as part of the Glitch Works 8085 SBC projects. These designs have been manufactured and tested and generally found to be functional; however, no warranty is made as to their fitness for any purpose. Please see the [LICENSE](https://github.com/glitchwrks/8085_sbc/blob/master/LICENSE) file for more information.

If you are interested in obtaining a bare circuit board, kit, or assembled board, please contact us through GitHub or [the Glitch Works contact form](http://www.glitchwrks.com/contact/index.html). There's a chance we'll already have a bare board on hand, since later boards were ordered through [OSH Park](https://oshpark.com/) and resulted in three boards.

If you decide to produce any of these designs, or assemble a board from the provided schematics, please let us know through GitHub or [the Glitch Works contact form](http://www.glitchwrks.com/contact/index.html).

### 8085 SBC rev 1

This is the original PC board produced from the "mess of wires" that started my exploration into the 8085 CPU! You can read more about the board's evolution and design [here](http://www.glitchwrks.com/2010/09/02/8085-sbc). This board was meant to be the CPU board in a stack of boards, and contains 8K EPROM, 8K static RAM, an 8085, and associated clock generation and memory decode circuitry. You can flash a LED on the SOD pin with nothing more than this basic hardware.

### 8085 SBC rev 2

An extension of the rev 1 design, this board incorporates more RAM and ROM, mounting holes, and a few other features. Read about the board [here](http://www.glitchwrks.com/2011/10/29/sbc-rev-2).

### I/O Board

Apparently I never did a write-up on this one! This board contains a Zilog SCC (two channel USART) and Intel 8255 PPA to provide two serial ports and 24 bits of parallel I/O. It stacks on top of the 8085 SBC board, PC-104 style. I wrote a [ROM monitor](https://github.com/chapmajs/glitchworks_monitor) that works with this board. This was on display at [HOPE Number Nine](http://hope.net/) with the vintage computer guys.