## 2nd-Year-Microcontroller-Project-

Implementation Of Full Adder Using Assembly Level Language





# Full Adder
Full Adder is the adder which adds three inputs and produces two outputs. The first two inputs are A and B and the third input is an input carry as C-IN. The output carry is designated as C-OUT and the normal output is designated as S which is SUM.
A full adder logic is designed in such a manner that can take eight inputs together to create a byte-wide adder and cascade the carry bit from one adder to the another.

---



## Circuit Diagram :-

<img src = "Circuit Diagram.png">






---




## Installation 


     1:Download arduino package for ubuntu:-https://www.arduino.cc/en/Guide/Linux
	  Follow this link for Arduinio installation and serial port permission

     2:Install AVRA and AVRDUDE:- sudo apt install avra avrdude

	This former converts the .asm file(code/scriptfile) to hex and the latter helps in uploading the .hex file to the micrcontroller.


     3:Download the m328Pdef.inc file from this link :-https://www.instructables.com/id/Command-Line-Assembly-Language-Programming-for-Ard/
	Include this library file in the first line of the source code

     4:Open a text editor and write the code in assembly language and save as .asm file

     5:Open the terminal:- 
	1) avra file.asm
	    This converts the file.asm to file.hex

        2) avrdude -C /etc/avrdude.conf -v -p atmega328p -c arduino -P /dev/ttyACM0 -b 115200 -D -U flash:w:/home/iiit/Downloads/        fwdassemblywitharduino/file.hex:i
	    This command uploads the file.hex to the flash memory
	    
      6) AVR Assembler Instructions:-
       https://www.microchip.com/webdoc/avrassembler/avrassembler.wb_instruction_list.html




---



## Implemented Diagram :-

<img src = "Implemented Diagram.png">




---

## Truth Table Of Full Adder

<img src = "Truth Table.jpg">




---

## Team Members :-

1.  Shantanu Tripathi ( 18BCS116 )
2.  Yashdeep Suresh Shetty ( 18BCS092 )
3.  Syed Sufyan Ahmed ( 18BCS103 )


---
