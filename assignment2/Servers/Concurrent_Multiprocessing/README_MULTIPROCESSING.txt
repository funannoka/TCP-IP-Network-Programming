This is the README file for Concurrent Multiprocessing server program using TCP and UDP protocol.

CONTENTS OF THE PACKAGE:

Folder name : tcp

tcpserver.c
errexit.c
passivesock.c
passiveTCP.c
test.txt
makefile

Folder name : udp

udpserver.c
errexit.c
passivesock.c
passiveUDP.c
text.txt
makefile

SYSTEM REQUIREMENTS:

LINUX OPERATING SYSTEM
GNU COMPILER

CODE COMPILATION:

>$ make

OUTPUT COMMAND:
>$ output

DESCRIPTION:

This program creates a file server at a given port. When a client requests a particular file which is in the server, the file is sent to the client using the port which is assigned.

The program has 4 modules.

tcpserver.c /udpserver.c : Main server program which uses UDP or TCP protocol to create a server at a specific port.
passivesock.c: Contains socket allocation details. It allocates either a datagram or a stream socket, binds the socket to the well-known port for the service and returns the socket descriptor to the caller.
passiveTCP.c /passiveUDP.c: Allocates a socket and bind it to a well-known port for a service.
errexit.c: Prints the error occurred and exits

EXAMPLE OUTPUT:

>$ ./output 5500

**port is opened for a client to access the file**
 

**When the file is not present in the server the following is displayed in client program**

Unable to copy. File does not exist in the server.



