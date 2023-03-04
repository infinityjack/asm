info:

section.data                   ;declare init data, buffer, 
                                ;filename, constant


section.bss                    ;declare variable


section.text                   ;save actual code, 
                                ;must start with 'global_start'
                                ;it is entry point of program

;comment, start with ';'

;this is a program displays a message on screen


add eax, ebx             ;add ebx to eax


assembly statements:
    executable instructions
    assembler directives or pseudo-ops, and macro


syntax:
    [label] mnemonic(zhujici) [operands]    [;comments]


e.g.:
    inc count     ;increment the memory variable count


    mov total, 48     ;transfer the 48 in the 
                        ;memory variable total

    add mask1, 128      ;perform and operation on the
                        ;variable mask1 and 128

    add masks, 10           ;add 10 to the variable masks

    mov al, 10              ;transfer the value 10 to the al register



memory segment:
    data seg
    bss seg
    stack seg


register:
    processor register:
        1.general reg:
            
            1.1.data reg:

                four 32 bit reg eax, ebx, ecx, edx, used for arithmetic,
                    logical, and other ops.
                
                lower halves of 32-bit can be used as 16-bit 
                    data register: ax, bx, cx, dx
                
                low and high halves of 16-bit can be used as 
                    eight 8-bit register:
                        ah, al, bh, bl, ch, cl, dh, dl
                
                ax(primary accumulator):
                    input, output arithmetical instructions.
                
                bx(base register):
                    indexing address

                cx(count register):
                    store the loop count

                dx(data register):
                    work with ax for large number operations
            

            1.2.pointer reg:

                3 32-bit pointer reg are eip, esp, ebp.

                corresponding 16-bit right portions ip, sp, and bp
                
                ip(instruction pointer):
                    16-bit reg stores offset addr of 
                        next instruction to be executed.

                    ip association with cs reg(cs: ip) gives 
                        the complete addr of current instruction
                            in the code seg

                sp(stack pointer):
                    16-bit reg provides the offset value with stack

                    sp association with ss reg(ss: sp) refers to be 
                        curr pos of data or addr with stack

                bp(base pointer):
                    16-bit reg helps in referencing the para variables
                        passed to a subroutine.

                    the addr in ss reg is combined with the offset in
                        bp to get loc of para.

                    bp can also combineed with di and si as base reg
                        for specical addressing


            1.3.index reg:

                2 32-bit index reg are esi and edi, their 16-bit 
                    rightmost portions, si, di are used in add
                        and sub.
                
                si(source index):
                    as src index for string ops

                di(destination index):
                    as dest index for string ops
                

        2.control reg:

            2.1. 32-bit instruction pointer reg and 32-bit flags reg 
                combined are cosidered as control reg.

            2.2.common flags:

                of(overflow flag):

                df(direction flag):

                if(interrupt flag):

                tf(trap flag):

                sf(sign flag):

                zf(zero flag):

                af(auxiliary carry flag):

                pf(parity flag):

                cf(carry flag):


        3.segment reg:
                
            cs(code seg):
                contains all instructions to be executed.

            ds(data seg):
                contains data, constants, and work area.

            es(extra seg):
                provides addtional addr of data seg.

            ss(stack seg):
                contains data and return addr of procedures
                    or subroutines.


