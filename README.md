# 16-Bit-Computer
Construction and working of a basic 16 Bit computer
List of circuits implemented in this construction :

● Control Unit (which coordinates all the signals, control functions,
bus selection, etc.)

● Bus control unit (which selects the register data to be loaded on
bus)

● Register control circuits (which tell which of the following (LOAD,
INCREMENT or CLEAR) operations are to be performed on which
register/s).

● Adder circuit : This circuit gives us a list of operations which can be
performed with the data present in the accumulator. This circuit is
made of two sub-components :
1. Adder stage : This gives us the bitwise operations between all
of the DR and AC bits.
2. Gate control structure : This control circuit selects which of
the operations is to be allowed to be sent to the AC.

● Sequence Counter CLEAR : This circuit clears the sequence counter
whenever the given instruction is completed.

All of the above sub-components are combined in the main circuit and
hence created the basic computer. The instruction length of the
micro-instruction is 12 bits and the operand length is 16 bits.
The overall size of the memory unit (RAM) in this computer is 4096 x 16
bits. The registers AR and PC have sizes 12 bits, as they store addresses of
instructions. The registers DR,AC,IR,TR have sizes of 16 bits, as they
store either memory words (operands) or instructions. However, the
registers AR and PC have 16 bits for this computer.
The input and output registers have 16 bits each as it would be
convenient to load them onto the MUX without difficulties.
