Most modern keypad microphones do not generate DTMF tones but rather generate a digital serial data stream that communicates keypress information to the host radio.  This project creates a small interposer PCB that re-purposes a commercially available micropohne (the KMC32 for Kenwood radios) allowing the microphone to generate DTMF tones directly.

To accomplish this, several components are removed from the microphone keypad PCB which allows the interposer to be seated into place allowing it to directly intercept the row, column, and GND pads on the keypad PCB.  The addition of a few small wires completes the connections.  Once reassembled, the modified microphone is able to generate DTMF tones on command.l

The HW folder describes the PCB and the modification instructions.  The SW folder describes the C source files for the ATTINY3217 MCU used to detect the keypresses and subsequently generate the DTMF tones using direct digital synthesis techniques.
