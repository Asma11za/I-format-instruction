<h1> Implementation of I-format instructions (Single Cycle Path)  </h1>

1. Step 1)
- Reg (2b) will fetch the instruction.
- An adder connected to it will help find the next instruction and fetch it.  

2. Step 2)

- 4b ROM (instruction memory) will decode and analyze the instruction.
  
3. Step 3)

- Register will fetch the operation (read Source 1 only), the other value will go through Sign Extend.    
4. Step 4)

- ALU will execute the I-format instruction and then write the result in the second 4b ROM.
- if the instruction is LW then write the result in the register, if SW then will not write the result in the register.  
