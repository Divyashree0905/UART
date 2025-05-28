# UART
Implementation of UART using Verilog code in Vivado and ISE 14.7
ART, or Universal Asynchronous Receiver/Transmitter, is a hardware module that facilitates asynchronous serial communication between devices. It converts parallel data into a serial stream and back, enabling data transfer over a simple two-wire connection. This process involves adding start, stop, and optionally parity bits to the data before transmission and then reconstructing the parallel data at the receiving end.


Key Concepts:
Asynchronous Communication:
Unlike synchronous communication, UART relies on start and stop bits to signal the beginning and end of data transmission, rather than a separate clock signal. 
Serial Data:
UART transmits data bit by bit, one bit at a time, in a serial fashion. 
Data Frame:
UART transmits data in frames, which typically include a start bit, data bits (usually 8 bits), an optional parity bit for error detection, and one or two stop bits. 
Baud Rate:
The baud rate defines the transmission speed of the serial data, measured in bits per second (bps). 
FIFO (First-In, First-Out):
UARTs often utilize FIFO buffers to temporarily store data before and after transmission, improving the efficiency of data transfer. 



UART Operation:
1. Transmission:
The transmitting UART receives parallel data from a data bus (like a CPU or microcontroller). 
2. Frame Formation:
The UART adds a start bit, data bits (8 bits by default), an optional parity bit, and stop bits to the data, forming a data frame. 
3. Serial Transmission:
The UART transmits the data frame bit by bit over a single wire. 
4. Reception:
The receiving UART receives the serial data bit by bit and reconstructs the parallel data by removing the start, parity, and stop bits. 
5. Parallel Data:
The receiving UART transfers the parallel data to the data bus at the receiving end.




Advantages of UART:
Simple and Cost-Effective: UART uses a minimal number of wires (two plus ground) for communication, making it cost-effective. 
Easy to Implement: UART is a straightforward protocol to implement in hardware and software. 
Widely Used: UART is a widely adopted serial communication protocol used in various applications, from basic serial communication to more complex systems. 




Applications of UART:
Serial communication between microcontrollers and peripherals .
Data logging and storage .
Connecting computer peripherals (e.g., mice, keyboards) to computers .
Networking and communication in embedded systems . 
