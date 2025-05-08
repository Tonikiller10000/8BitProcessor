# 8Bit Computer/ Processor_ALU

<table>
  <tr>
    <td>

### Description:
This board is used for addition and substraction. It is formed of 2 registers A and B, the actual ALU (Arithmetic and Logic Unit), and the Flag Register witch has a Carry flag, a Zero flag, a Sign flag and 5 other empty, free to use for other stuff, flags. 
    </td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(6).png"/></td>
  </tr>
 </table>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(5).png"/>



### How to use:
1. Put values in the A and B register by putting a value on the bus and setting the A_IN or B_IN pin HIGH.
2. By setting the SUB pin LOW (default), the ALU adds the A Reg value and the B reg Value upt to 255, 
after witch the carry flag gets activated and the result remain the difference between the result and 256.
EX. 199 + 69 = 22(+C)
When the SUB pin is pulled HIGH, the ALU returns the difference between A register value and B register value.
3. The carry input can be changed from the C_IN pin.
4. By setting the F_IN pin HIGH, the flag values are saved in the Flag register. 
5. The result of the ALU can be outputed in the bus by putting the ALU_OUT pin HIGH.
The ALU result can be put back in the A or B registers and be used for other operations.

<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(18).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(11).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(12).jpg"/></td>
  </tr>
 </table>

### How it wworks
The A and B registers are dmade with an 8 bit register with output always enabled and an tristate buffer to connect the register to the buss. By making it this way, you can always see the internal value on the led\`s and the register values are continuousely sent to the ALU. The 8 bit adder is made of 2x 4bit adders, and the substraction is made by inverting the bits values of the B register. By inverting the B register bits values, the value in the B register is negate and by adding the negative of a number, you can substract it: 
<br><b> 3 + (-2) = 1 </b><br>
The inversion of the B register bits is made with an NAND gate witch can be made as an enable pin.




### Mentions:
- All the pins should have an pull-down resistors to assure the default mode opperation
- By not using resistors for the led\`s thinking that the 74LSx series IC\`s has integrated resistors, the led\`s are to brigth, and their intensity changes depending on how many led\`s are ligthned up. ( https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(17).jpg )
- This is the first version, Future versions will come in the next version of the processor. ( https://github.com/Tonikiller10000/8BitProcessor/tree/main )
- It can make more complex opperations like, multiplication(repeated addition), division(repeated substraction) and rise to power(repeated multiplication) with the rigth software 
- The 74LS574 IC is the same as the 74LS374 IC but has a different pinnout witch makes it easier to use
- The 74LS573 and 74LS373 are the same as the 74LS574 and 74LS374, but the latching time happends on the entire length of the HIGH clk pulse.

Datasheets:
- 74LS245 (Tri-state buffer): https://pdf1.alldatasheet.com/datasheet-pdf/view/51057/FAIRCHILD/74LS245.html
- 74LS574 (8 bit register): https://pdf1.alldatasheet.com/datasheet-pdf/view/51086/FAIRCHILD/74LS574.html
- 74LS283 (4 bit adder): https://pdf1.alldatasheet.com/datasheet-pdf/view/8069/NSC/74LS283.html
- 74LS86 (4x XOR gate): https://pdf1.alldatasheet.com/datasheet-pdf/view/51095/FAIRCHILD/74LS86.html


74LS00: https://pdf1.alldatasheet.com/datasheet-pdf/view/51021/FAIRCHILD/74LS00.html 
74LS283: https://pdf1.alldatasheet.com/datasheet-pdf/view/1718878/ETC1/74LS283N.htm
74LS374: https://pdf1.alldatasheet.com/datasheet-pdf/view/51080/FAIRCHILD/74LS374.html 
74LS245: https://pdf1.alldatasheet.com/datasheet-pdf/view/12640/ONSEMI/74LS245.html 
