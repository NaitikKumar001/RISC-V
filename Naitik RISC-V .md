# 1. INTRODUCTION 

This repository contains my notes, examples,
while learning RISC-V.
The goal is to understand how RISC-V works
as an Instruction Set Architecture (ISA) 
and how its instructions are used in programs.


# 2. WHAT IS RISC-V?
   
RISC-V is an open-standard Instruction Set Architecture(ISA).It defines the instructions and rules that a processor can understand.RISC-V is not a processor 
or a programming language. It is an Instruction Set Architecture.It is a Set of rules that tells a CPU which instructions it can understand and how 
those instructions work.
           <pre>
       RISC-V is not processor itself
                 RISC-V
                    |
        INSTRUCTION SET ARCHITECTURE
                    |
          DEFINES INSTRUCTIONS AND RULES
                    |
      DIFFERENT COMPANIES CAN BUILD CPUs USING
                  THOSE RULES
</pre>

# 3. EASY UNDERSTANDING.

Let,RISC-V as a rule book In which all things aremmentioned that "how CPU understand instructions","how to decode instructions","how to execute
instructions",RISC-V tells the CPU how to Handel instructions.
we also decide how many instructions to give to which device and how many not to give. 

# 4. ORIGIN OF RISC-V.

RISC-V is an open standard ISA based on RISC design philosophy."It was developed primarily at the university of California,Berkeley.

# 5. WHY WAS RISC-V CREATED?

Around 2010,researchers at California wanted a ISA that could be:
.Free to use
.Open and accessible 
.Suitable for research and education 
.EASY to modify according to processor design
.Not controlled by single company

Then researchers introduce RISC-V which is an open standard ISA which carry these all property mentioned above. Now, if any one want to designe it's own processor,it has no need to make a complete different ISA it can designe it's processor based on RISC-V. 
In current time companies make there CPUs,GPUs based on RISC-V. 
RISC-> REDUCED INSTRUCTION SET COMPUTER 
V-> V means "five". 
It is a fifth major RISC ISA design in university of California. 

# 6. REGISTERS USE IN RISC-V.

We all know to fetch,to decode,to execute instructions we need registers. 
RISC-V has 32 registers "x0-x31" each has 32 bit wide storage .simply treat each register as a box in which address of your instructions stored.
there is a "special register which is x0" because it contains only 0.

# 7. HOW RISC-V WORKS?

RISC-V works by defining a set of instructions that a processor can understand and execute. A program is converted into RISC-V instructions, which tell the CPU what operations to perform, such as adding numbers, moving data, accessing memory, or making decisions. The processor fetches these instructions from memory, decodes them, and then executes them step by step. RISC-V defines what instructions do, while the actual processor is responsible for implementing those instructions.

# 8. CLOCK SPEED (FREQUENCY).

clock speed indicates how many instructions cycles that processor can attempt per second.
NOTE-> Higher clock speed can't always means faster performance. 

| Frequency | Cycles Per Second | Typical Usage |
|-----------|-------------------|---------------|
| 1 MHz     | 1 million         | Early (1970s) |
| 100 MHz   | 100 million       | Basic embedded systems |
| 1 GHz     | 1 billion         | Smartphones, tablets |
| 3 GHz     | 3 billion         | Desktop computers |
 
| Processor Type | Instructions per Cycle |
|----------------|------------------------|
| Simple Processor | 1 instruction per cycle |
| Superscalar Processor | 2–4 instructions per cycle |
| High-Performance Processor | 4–8 instructions per cycle |


# 9. What is ISA?

**ISA (Instruction Set Architecture)** is a set of rules and specifications that defines how software communicates with a CPU. It acts as a bridge between **software and hardware**.

An ISA defines:

- The instructions a CPU can understand, such as `ADD`, `SUB`, `AND`, `OR`, and `LOAD`.
- The registers available to programs.
- The data types and sizes the processor can work with.
- How memory is accessed.
- How instructions are represented in machine code.
- What each instruction does when executed.

For example:
ADD x5, x6, x7
so ISA tells to processor what is add operation how to perform it what are x5,x6,x7 and how to encode them in binary.

          
