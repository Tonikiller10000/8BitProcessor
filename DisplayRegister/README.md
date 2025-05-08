# 8Bit Computer/ Display Register

### Description:
This board is an 8 bit register witch can display it\`s value on an 4 digit 7 segment display using the multiplexing process. It has 8 led\`s to display it\s contents in binnary, an 2 position switch to help you select between 2 programable modes (HEX, DEC, SGN_DEC, ...) and a potentiometer to increase/decrease the multiplexing speed to help understanding of the multiplexing principle. 


<table>
  <tr>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/pr3.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/pr1.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/pr2.png/></td>
  </tr>
 </table>
Schematic:
<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/sch.png/>






### How it works
The 8 bit bus is connected to the 74LS574 8 bit register witch outputs it\`s value to 8 address pins of the EEPROM  and to the led\`s to show it\`s value.
Another 2 EEPROM address pins are used to select one of the 4 digits value, and the rest are connected to switches to select the displaing mode (EX. negative numbers) or tied to 0V or 5V if not used.
The display is connected to an demultiplexer(74LS138) witch selects witch digit to be displayed, and the demultiplexer with the eeprom are connected to a binnary counter made with 2 JK latches(74LS76) witch recive clk pulses from an NE555 timer IC. The clk speed can be changed from the potentiometer to admire the multiplexing effect.




<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/pic1.jpg/>
<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/DisplayRegister/DisplayRegister_Pictures/pic4.png/>



### Results:
Power it to 5V, put a value on the bus, store it by setting the D_in pin HIGH and every thing should work.
The project is working, but the frequency interval of the potentiometer wasn\`t verry visible, so the capacitors and resistors values should be changed. 


Datasheets:
- 74LS574 (8 bit register): https://pdf1.alldatasheet.com/datasheet-pdf/view/51086/FAIRCHILD/74LS574.html
- AT28C64 (8K x 8 EERPOM): https://pdf1.alldatasheet.com/datasheet-pdf/view/157137/ATMEL/AT28C64.html
- AT28C256 (32K x 8 EERPOM): https://ww1.microchip.com/downloads/en/DeviceDoc/doc0006.pdf
- 74LS138 ( 3 -> 8 demultiplexer ): https://pdf1.alldatasheet.com/datasheet-pdf/view/51039/FAIRCHILD/74LS138.html
- 74LS76 (JK Flip Flop): https://pdf1.alldatasheet.com/datasheet-pdf/view/12663/ONSEMI/74LS76.html
- NE555: https://pdf1.alldatasheet.com/datasheet-pdf/view/471200/STMICROELECTRONICS/NE555.html








