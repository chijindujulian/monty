# 0x19. C - Stacks, Queues - LIFO, FIFO
---
![Tea](https://https://github.com/chijindujulian/monty/blob/master/src/makeTea.png)

### Description
This is an ALX project to create a custom ByteCode interpreter for the Monty Language, developed in C.

## The Monty Language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

### Monty Byte Code Files
Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:

```push 0$
push 1$
push 2$
  push 3$
                   pall    $
push 4$
    push 5    $
      push    6        $
pall$

Monty byte code files can contain blank lines (empty or made of spaces only, and any additional text after the opcode or its required argument is not taken into account:

```
push 0 Push 0 onto the stack$
push 1 Push 1 onto the stack$
$
push 2$
  push 3$
                   pall    $
$
$
                           $
push 4$
$
    push 5    $
      push    6        $
$

## Usage
---
All the files are compiled in the following form:
```gcc -Wall -Werror -Wextra -pedantic *.c -o monty.

To run the program

```
./monty bytecode_file
