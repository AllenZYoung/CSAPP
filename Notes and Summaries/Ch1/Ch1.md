# Ch.1 A Tour of Computer Systems
This chapter introduces the major
ideas and themes in computer systems by tracing the life cycle of a simple
“hello, world” program.

Since chapter 1 is just a brief introduction to some vital concepts in this book, my summary is 
brief, too.

## 1.1 Information Is Bits + Context
<br>
The source program (saved in a text file called xxx.c) is a sequence of bits, each with a value of 0 or 1,**organized in 8-bit chunks called bytes**.  *This is a very useful and significant concept.*<br>
In different **contexts**, the same sequence of bytes
might represent different things.

## 1.2  Programs Are Translated by Other Programs into Different Forms

Object programs are also referred to as **executable object files**.<br>
The translation from source file to object file is performed by a ***compiler***.
<br>chunk
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
<br>
![fig-1.4.png](https://ooo.0o0.ooo/2015/12/17/567360696213c.png)
### Buses
Buses are typically designed to transfer fixed-sized chunks of bytes known as **words**. The
number of bytes in a word (the *word size*) is a fundamental system parameter that
varies across systems. Most machines today have word sizes of either **4 bytes (32
bits) or 8 bytes (64 bits)**.
### Main memory
The *main memory* is a temporary storage device that holds both a program and
the data it manipulates while the processor is executing the program. Physically,
main memory consists of a collection of *dynamic random access memory* (**DRAM**)
chips.
### Processor
The *central processing unit* (**CPU**), or simply *processor*, is the engine that interprets
(or executes) instructions stored in main memory. At its core is a word-sized
storage device (or register) called the *program counter* (**PC**). At any point in time,
the PC points at (contains the address of) some machine-language instruction in
main memory.

## 1.5 Cashes matter
To deal with the processor-memory gap, system designers include smaller
faster storage devices called *cache memories* (or simply **caches**) that serve as
temporary staging areas for information that the processor is likely to need in
the near future. <br>
By setting up caches to hold
data that is likely to be accessed often, we can perform most memory operations
using the fast caches.

## 1.6 Storage Devices Form a Hierarchy
<br>
![fig-1.9.png](https://ooo.0o0.ooo/2015/12/17/5673639c95f0b.png)
## 1.7  The Operating System Manages the Hardware
Some significant concepts:

- **Processes**: the operating system
provides the illusion that the program is the only one running on the system.
- **Context switching**: The operating system performs this interleaving
with a mechanism known as context switching.
![fig-1.12.png](https://ooo.0o0.ooo/2015/12/17/56736503397ea.png)
- **Threads**: in modern
systems a process can actually consist of multiple execution units, called threads.
- **Virtual memory**:  an abstraction, provides *virtual address space* for processes.
![FIG-1.13.png](https://ooo.0o0.ooo/2015/12/17/56736660c52f1.png)
- **Files**: A sequence of bytes. Every I/O device,
including disks, keyboards, displays, and even networks, is modeled as a file.

## 1.8 Systems Communicate with Other Systems Using Networks
## 1.9 Important Themes.
- [Concurrency](https://en.wikipedia.org/wiki/Concurrency_(computer_science)) and [Parallelism](https://en.wikipedia.org/wiki/Parallel_computing).
- Abstractions in Computer Systems.
![fig-1.18.png](https://ooo.0o0.ooo/2015/12/17/56736806de54c.png)





 



