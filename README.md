# RISC-Assembly-Instruction-Decoder
I was shown a simple RISC machine and given the task to write code to decode the different assembly instructions to be passed to the machine to handle and manipulate data accordingly. It should be worth noting that this RISC machine, named the OSIAC machine, was designed and used by The Ohio State University. I was simply given the task of properly handling instructructions passed onto the machine.

Included along with the code, is a pdf explaining the functionality of the RISC machine which was being worked on. Along with the pdf. I will summarize the functionality below in order to explain what is possible with the instruction decoder I have written.

This machine has a 16-bit word-addressable memory. It has four available registers: AC acts as an accumulator for the machine, X is used as an index register, SP is the machine's stack pointer, and PC acts as the program counter. Their codes are 00, 01, 10, and 11 respectively. The machine also has four condition code bits available to the user: C, V, Z, and N. These condition bits are automatically manipulated to show specific conditions during calculations made on the machine. C represents a carry out bit, V represents that there is overflow in the calculation, Z indicates the result is zero, and N indicates the result is negative. 

There are additionally several invisible registers: MAR, MDR, IR, T1-T5, and Q. MAR represents the Memory Address Register, which holds the address of the data which is being manipulated, and MDR represents the Memory Data Register which holds the actual data that is being manipulated. IR is the Instruction Register which holds the 16 bit instruction that is currently being executed on the RISC machine. T1-T5 are general registers used to hold onto data when not currently being used. Finally, Q is used as a register to hold the result of any calculations performed on the machine.

The machine accepts sevel different addressing modes: Register addressing, Register Indirect addressing, Autoincrement addressing, Autodecrement addressing, Index addressing, Absolute addressing, and Immediate addressing. 

Some of the instructructions that can be performed on this machine include but are not limited to single operand instructions such as Clear, Increment, Decrement, Negate, Complement, Jump, and Jump to Subroutine. This machine may also perform double operand instructions such as Add, Subtract, Move, Exchange, OR and AND instructions. 

For additional explanation on the function of the RISC machine, please refer to OSIAC_Description.pdf. As previously stated, I am not the designer of this RISC machine. I simply supplied my own code to handle these instructions properly given the limitations of the state machine.
