
work: 
1. open a connection 
2. send and recieve raw bytes
3. handle disconnects 

N.B: a bit torrent peer connection or communiccation is all TCP 


network socket
----------
as example we can say that one website is actually rrunning on an ip 100.10.1.11 then the socket  number or the socket IP would be 100.10.1.111:80

sockets can be classified into two types and they are stream socket and the other one is datagram socket they are portraied by socket.SOCK_STREAM and socket.SOCK_DGRAM

- SOCK_STREAM is mainly associated with the TCP protocol and this is meant to provide security in the transmission of data and the sequence of the data, but on ther other hand 
- SOCK_DGRAM is mainly associated with UDP protocol where that does not actuaaly care about the security of the transsferred data rather ot shows that the packets will go over on a datagram type. which has a asynchronious communication stype 

introduction to TCP socket 
----------
TCP socket is actually a transmission oriented socket that depends on the transmission control protocol. they require the packets connection to be based on the three way handhsake protocoll containing the SYN, SYN-ACK and ACK package. they also gurantee that the data is actually recieved and acknoledged by the client to the server or vice versa because this is actually a two way protocol 

For example, we are sending an HTTP request from our client at 120.1.1.1 to the website at 189.1.1.1. The server for that website will use well-known port number 80, so its socket is 189.1.1.1:80, as we saw before. we have been ephemeral port number 3022 for the web browser, so the client socket is 120.1.1.1:3022. The overall connection between these devices can be described using this socket pair: (189.1.1.1:80, 120.1.1.1:3022).

advantages
----------
- reliable 
- in order data delivery 

how to open a connection, TCP socket
---------
just mention that how the hell actually the TCP/IP 3 way handshake works and that is exactly how we extablish a tco connection and send data over that 

TCP connection termination 
----------
1. abrupt connection release - one of the entities are actually forsed to close the conntion and that makes the connection between the two entities in the network loose the conection 
2. gracefull connection release - where the connection release is done by both of the entities and they come to a conclution that the data transfer is actually done any they need to release the connection because there is no more need of data transfer between them, no force closing rathe closing the connection with a mutual understanding 

