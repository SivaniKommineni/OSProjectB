# OSProjectB
This project focuses on implementing system calls in an operating system. Created system calls for printing strings to the video, reading input from the keyboard, and reading disk sectors. Created printString(char*)  function to take a character array and print each character until it encountered the null character (0x0). Created a readString function,  that reads characters from the keyboard and also handles backspace (ASCII 0x08) for editing. Created a readSector(char* buffer, int sector) function that reads a disk sector into a character array. Also created an interrupt handler (handleInterrupt21), specifically for interrupt 0x21. Modified the interrupt 0x21 handler to provide services for printString, readString, and readSector. Defined how each function should be called based on the value in AX.
‘compileOS.sh’ is used to run all the comments. Command java -jar simulator.jar is given to start the stimulator. 

The following functionalities have been successfully implemented:

Displaying content on the screen.

Reading characters from the keyboard

Read a sector from the disk

Implementing interrupt.

Interrupt 0x21 handler providing printString, readString, and readSector services.
