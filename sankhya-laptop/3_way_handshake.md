so then tcp/IP 3 way handshake is performed to make sure that the connection is atable and the file transfer can happen smmoothly between the server and the client. 
so what happens in the handshake protoccol is written in ther following 

1. the client is going yo send the ISN(initial sequence number) to the server inside of an SYN packet 
2. after recieving that packet the server is actuaaly going to see the packet and ackneledge that ffor the upcoming transaction and setds that acknoledgement trough using a SYN-ACK packet
3. then ther client sends over the final ACK packet so the server knoes that the last sent packet was acknoledged by the client 

and after that the secure client server communication is actually extablished sopp then the the client and the server can actually send over recieve data over the built in conneciton. 

