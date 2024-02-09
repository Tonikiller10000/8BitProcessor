# 8Bit Computer/ Processor_ALU

### Description:
This board is used for addition and substraction. It is formed of 2 registers A and B, the actual ALU (Arithmetic and Logic Unit), and the Flag Register. 

### How to use:
First, put values in the A and B register by putting a value on the bus and setting the A_IN or B_IN pin HIGH. By default, the ALU adds the A Reg value and the B reg Value upt to 255, after witch the carry flag gets activated and the result remain the difference between the result and 256.
EX. 199 + 69 = 22(+C)
By setting the SUB pin HIGH, the ALU returns the difference between A register value and B register value.
!!! carry flag ....
By setting the F_IN pin HIGH, the flag values can be saved in the Flag register. This action sets all the flag values with the corresponding value at that time.  
After the operation mode is set from the SUB pin and the flags are saved in the Flag register (optional), the result of the operation can be outputed in the bus by putting the ALU_OUT pin HIGH. From the bus, the result can be put back in the A or B registers without crating a loop, the registers beeing clk edge enable.

> [!TIP] All the pins should have an pull-down resistors to assure the default mode opperation.

-----

[!TIP] All the pins should have an pull-down resistors to assure the default mode opperation.


### Features:
- Fast addition and substraction opperations;
- A & B registers free to use for other operations;
- Flag register with Carry flag, Zero flag, Sign flag and 5 other empty, free to use flags;
- Frendly user interface and good educational visual interface.







<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(1).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(2).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(2).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(3).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(3).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(4).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(4).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(5).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(5).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(6).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(6).png"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(7).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(8).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(9).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(10).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(11).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(12).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(13).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(14).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(15).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(16).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(17).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(18).jpg"/>
<img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(19).jpg"/>






Datasheets:
- NE555: https://pdf1.alldatasheet.com/datasheet-pdf/view/471200/STMICROELECTRONICS/NE555.html
- 74LS00 (4x NAND gate): https://pdf1.alldatasheet.com/datasheet-pdf/view/51021/FAIRCHILD/74LS00.html 



