# modi-SIC-DIASSEMBLER-PROJECT
A modi-SIC disassembler is a program that translates machine code (HTE record) into an assembly code for the Modified Simplified Instructional Computer (modi-SIC).

The modi-SIC consists of
1. Same instructions set (Format 3) of SIC
2. Same idea of reservation of variables in memory using BYTE, WORD, RESB, RESW

modi-SIC is extened to include
1. Format 1 instuctions
2. Immediate Instruction (Format 3) that deals with an immediate value passed to as integer.
For the sack of simplification a list of modi-SIC instructions is attached at the end of project description that
have all instructions handled by modi-SIC + a full description of a new introduced bit that states if the
instruction is dealing with immediate or not.

It takes as an input a text file (in.txt) that contains modi-SIC machine code (modi-SIC HTE record).
Remember that The modi-SIC HTE record will be modified to accept also object code of Format 1 instruction of
SIC/XE. So this case must be handled.

it generates a symbol table file (symbolTable.txt) for all the
symbols extracted from the HTE record.

it generates the assembly code file (assembly.txt). It must contain three columns ordered from left
as location counter, the assembly code, and object code.
