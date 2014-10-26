8bitALU
=======

Multisim PLD files for 8-bit ALU implemented with carry look-ahead adder, shifter, comparator, Boolean module, and multiplier.

The ALU accepts 2 8-bit inputs A and B, and its functionality and 8-bit output is controlled by a 6-bit input ALUFN.


## ALU.ms12

ALU.ms12 is the overall ALU file. In it contains all five modules: adder, shifter, comparator, Boolean module, and multiplier.

The output from each module is hooked up to a series of multiplexers, which, depending on ALUFN, will select the appropriate final output.

The second bit of ALUFN controls the 2-to-1 mutliplexer, which selects from the adder (0) and multiplier (1) outputs.

The last two bits of ALUFN, bit 5 and 6, control the 4-to-1 multiplexer, which selects from the 2-to-1 multiplexer output (00) , the Boolean module output (01), the shifter output (10), and the comparator output (11).

## 8BITADDERSUB.ms12

This is the overall module for the 8-bit carry look-ahead carry.

### 

## BOOLEAN.ms12

## Shifter.ms12

This is the overall module for the 8-bit shifter, which is capable of logical left shifts, logical right shifts, and arithmetic right shifts of up to 7 bits.

## Comparator.ms12




