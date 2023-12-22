# 8Bit Computer/ Clock Pulse Generator

### Description:
This board generates 0-5V square wave CLK pulses for my 8Bit processor/computer and has an tactile switch to change between it\`s 2 states:
- astable mode: generate CLK pulses at variable speed by the potentiometer value from one pulse at every 1,2 seconds to an pulse at each every few milisecondes (The potentiometer and capacitor values should be changed)
- monostable mode: send debounced CLK signals at the push of a button

<table>
  <tr>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/p1.jpg/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/p2.jpg/></td>
  </tr>
 </table>

### PINS:
- VCC - 5V input
- GND - 0V input
- GND - 0V input (optional)
- HLT - input, connect to 5V to stop sending CLK pulses, and to 0V for normal operration
- CLK - CLK pulse generator output
- CLK - inverted CLK pulse generator output   //clk bar

<img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/d1.png/>

<table>
  <tr>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s1.png height=300/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s2.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s3.png/></td>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s4.png/></td>
  </tr>
 </table>

<table>
  <tr>
    <td><img src=https://github.com/Tonikiller10000/8BitProcessor/blob/main/ClkPulseGenerator/ComputerClk_Pictures/s.png height=400/></td>
    <td>
        This is the Ben Eater schematic made by me.
        https://youtu.be/SmQ5K7UQPMM?si=6SvCCjpXzhz8pTbt
    </td>
  </tr>
 </table>


Datasheets:
- NE555: https://pdf1.alldatasheet.com/datasheet-pdf/view/471200/STMICROELECTRONICS/NE555.html
- 74LS00 (4x NAND gate): https://pdf1.alldatasheet.com/datasheet-pdf/view/51021/FAIRCHILD/74LS00.html 



