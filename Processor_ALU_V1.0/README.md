# 8Bit Computer/ Processor_ALU



<table>
  <tr>
  <td>

### Description:
- This board is used for addition and substraction. It is formed of 2 registers A and B, the actual ALU (Arithmetic and Logic Unit), and the Flag Register. 

### Features:
- Fast addition and substraction opperations;
- A & B registers free to use for other operations;
- Flag register with Carry flag, Zero flag, Sign flag and 5 other empty, free to use flags;
- Frendly user interface and good educational visual interface.
    <td></td>
    <td> <img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(6).png"/> </td>
  </tr>
 </table>










> [!NOTE] 
> All the pins should have an pull-down resistors to assure the default mode opperation.


Board:
<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(18).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(11).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(12).jpg"/></td>
  </tr>
 </table>
Schematic:
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(5).png"/>



### How to use:
First, put values in the A and B register by putting a value on the bus and setting the A_IN or B_IN pin HIGH. By default, the ALU adds the A Reg value and the B reg Value upt to 255, after witch the carry flag gets activated and the result remain the difference between the result and 256.
EX. 199 + 69 = 22(+C)
By setting the SUB pin HIGH, the ALU returns the difference between A register value and B register value.
!!! carry flag ....
By setting the F_IN pin HIGH, the flag values can be saved in the Flag register. This action sets all the flag values with the corresponding value at that time.  
After the operation mode is set from the SUB pin and the flags are saved in the Flag register (optional), the result of the operation can be outputed in the bus by putting the ALU_OUT pin HIGH. From the bus, the result can be put back in the A or B registers without crating a loop, the registers beeing clk edge enable.



### Mentions:
- By not using resistors for the led\`s thinking that the 74LSx series IC\`s has integrated resistors, the led\`s are to brigth, and their intensity changes depending on how many led\`s are ligthned up. ( https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(17).jpg )
- 

Datasheets:
- 

