
The MIT License (MIT)

Copyright (c) 2014 Alex Smith <aosmith@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


toy-os
======
This is a toy operating system.  Right now it sets up the gdt and switches from real to protected mode.

Running:
--------
You can build and run this project with `make start`.

I've been running this using bochs, so it includes a bochsrc.txt.

Right now this boots to protected mode and runs main from `kernel.c`.  This just prints an X at the top left corner.

Useful commands:
----------------
Build:
`make all`

Run:
`make run`

Clean:
`make clean`

Reset:
`make reset`

Dump an object file:
`objdump -d basic.o`

Dissassemble Binary:
`nadisasm -b 32 basic.bin > basic.dis`

Compatibility:
--------------
Right now this should work on most linux systems (assuming you have nasm, gcc, ld, bochs, etc.).

What's the Point?
-----------------
This is simply the best way to learn about a computer on a very low level.  Getting to the point of booting and running c code is short but complex, this is a springboard / reference.




Based on "Writing a Simple Operating System -- from Scratch" by Nick Blundell.
