The first program FIFO1 generates an array of 50 random strings (of characters) of fixed length 5 each.
FIFO1 then sends a group of five consecutive elements of the array of strings to FIFO2 along with the 
ID’s of the strings, where the ID is the index of the array corresponding to the string. The second 
program FIFO2 accepts the received strings, and sends back the highest ID received back to FIFO1 to
acknowledge the strings received. The program P2 simply prints the ID’s and the strings on the console.
On receiving the acknowledged packet, FIFO1 sends the next five strings, with the string elements starting
from the successor of the acknowledged ID. Function sub_time is used to find the time taki=en by the process
in (seconds.nano_seconds) format.

The above mechanism has been implemented using FIFOs.
