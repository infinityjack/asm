# install nasm compiler:
#       sudo apt-get install nasm


1. create new file :
    example.s or example.asm

2. compile use nasm :
    nasm -f elf64 example.s

3. link it and create exe file:
    ld example.o -o example.exe

4. execute with : 
    ./example.exe
