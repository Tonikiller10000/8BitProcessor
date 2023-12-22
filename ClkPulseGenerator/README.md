# 8Bit Computer/ Clock Pulse Generator


<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/p1.jpg/>
<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/p2.jpg/>
<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s.png/>
<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/d1.png/>


<table>
  <tr>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s1.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s2.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s3.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s4.png/></td>
  </tr>
 </table>
Description:
This board generates the CLK pulses for my 8Bit processor/computer and has an tactile switch to change between it\`s 2 states.
In first mode, an NE555 timer in astable mode, generate the CLK pulses at an speed witch can be changed from the potentiometer from one pulse at every 1,2 seconds to an pulse at each every few milisecondes
(The potentiometer and capacitor values should be changed), and in the second mode, another NE555 timer in monostable mode to send debounced CLK signals at the push of a button

Pins:
- VCC - 5V input
- GND - 0V input
- GND - 0V input (optional)
- HLT - input, connect to 5V to stop sending CLK pulses, and to 0V for normal operration
- CLK - CLK pulse generator output
- CLK - inverted CLK pulse generator output   //clk bar

Links:
NE555: https://pdf1.alldatasheet.com/datasheet-pdf/view/471200/STMICROELECTRONICS/NE555.html
74LS00 (4x NAND gate): https://pdf1.alldatasheet.com/datasheet-pdf/view/51021/FAIRCHILD/74LS00.html
Inspired by Ben Eater Breadboard CLK: https://youtu.be/SmQ5K7UQPMM?si=6SvCCjpXzhz8pTbt



