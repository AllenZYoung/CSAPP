# Ch.1 A Tour of Computer Systems
This chapter introduces the major
ideas and themes in computer systems by tracing the life cycle of a simple
“hello, world” program.
## 1.1 Information Is Bits + Context
<br>
The source program (saved in a text file called xxx.c) is a sequence of bits, each with a value of 0 or 1,**organized in 8-bit chunks called bytes**.<br>
In different **contexts**, the same sequence of bytes
might represent different things.

## 1.2  Programs Are Translated by Other Programs into Different Forms
 The translation from source file to object file is performed by a **compiler**.
<br>
![fig1.png](https://ooo.0o0.ooo/2015/12/15/5670b9cdac7f3.png)
The programs that perform the four phases: 
**preprocessor, compiler, assembler, and linker**, are known collectively as the
**compilation system**.

## 1.3 It Pays to Understand How Compilation Systems Work
<br>
Some important reasons why programmers need to understand how compilation systems work:

- Optimizing program performance.(make program more efficient.)
- Understanding link-time errors.
- Avoiding security holes.(like buffer overflow vulnerabilities.)

## 1.4 Processors Read and Interpret Instructions Stored in Memory



