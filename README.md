# SAP---Simple-As-Possible
A model of the Simple as Possible CPU model

It starts with the "AUTO" switch in manual mode.
click on the "CLEAR" switch and then click the "STEP" button twice to zero out the program counter and the step counter.
click on the "RAM" chip to enter your program into the 16 addresses.
Then click on the "AUTO" switch to begin execution.

The HLT instruction will latch the CPU with the clock disabled.
You will need to click the "AUTO" switch to manual mode again, then hit "RESET" and "CLEAR" to set the unit for another run.

The instructions are in a 2 nybble format, the first nybble is the opcode and the second nybble is the argument.

opcodes
0H = NOP
1H = LDA (load A from argument address)
2H = ADD (add to A from argument address)
3H = SUB (subtract from A from argument address)
4H = STA (store A to argument address)
5H = LDI (load A with argument (immediate) value)
6H = JMP (jump to argument address)
7H = JC  (jump to argument address if carry flag is 1)
8H = JZ  (jump to agrument address is zero flag is 1)
EH = OUT (write A to output register to display bits on LEDs)
FH = HLT (latch the clock in a disabled state.  Can be cleared by hitting the "RESET" button)

