# Glitch Works 8085 SBC

This repository contains the recovered EAGLE projects for the various PC boards designed as part of the Glitch Works 8085 SBC projects. These designs have been manufactured and tested and generally found to be functional; however, no warranty is made as to their fitness for any purpose. Please see the [LICENSE](https://github.com/glitchwrks/8085_sbc/blob/master/LICENSE) file for more information.

If you are interested in obtaining a bare circuit board, kit, or assembled board, please contact us through GitHub or [the Glitch Works contact form](https://services.theglitchworks.net/ng/messages/new). There's a chance we'll already have a bare board on hand, since later boards were ordered through [OSH Park](https://oshpark.com/) and resulted in three boards.

If you decide to produce any of these designs, or assemble a board from the provided schematics, please let us know through GitHub or [the Glitch Works contact form](https://services.theglitchworks.net/ng/messages/new).

### 8085 SBC rev 1

This is the original PC board produced from the "mess of wires" that started my exploration into the 8085 CPU! You can read more about the board's evolution and design [here](http://users.glitchwrks.com/~glitch/2010/09/02/8085-sbc). This board was meant to be the CPU board in a stack of boards, and contains 8K EPROM, 8K static RAM, an 8085, and associated clock generation and memory decode circuitry. You can flash a LED on the SOD pin with nothing more than this basic hardware.

### 8085 SBC rev 2

An extension of the rev 1 design, this board incorporates more RAM and ROM, mounting holes, and a few other features. Read about the board [here](http://users.glitchwrks.com/~glitch/2011/10/29/sbc-rev-2).

[AN0001 describes ROM jumpers](https://github.com/glitchwrks/8085_sbc/blob/master/8085_sbc_rev2/an0001_jumpers.txt) for socket IC3.

### I/O Board

This board contains a Zilog SCC (two channel USART) and Intel 8255 PPI to provide two serial ports and 24 bits of parallel I/O. It stacks on top of the 8085 SBC board, PC-104 style. Read about design and testing [here](http://users.glitchwrks.com/~glitch/2017/04/24/8085-io-board). I wrote a [ROM monitor](https://github.com/glitchwrks/gwmon-80) that works with this board. This was on display at [HOPE Number Nine](http://hope.net/) with the vintage computer guys.

There's an [ECO for old etches](https://github.com/glitchwrks/8085_sbc/blob/master/io_board/eco0007.txt) that is relevant if you got one of these boards from us before 2023. It corrects a routing error w.r.t. the 8255 PPI reset signal. See the linked writeup above for a picture documenting the fix.
