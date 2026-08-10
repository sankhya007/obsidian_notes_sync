acronym
--------------------
TCP - transmission control protocol 
UDP - user datagram protocol
connections: 
--------------------
TCP - this iss actually a conncction oriented protocol meanis that the connnection needs to be ectablished before any data transfer is actually happenning in ther network 
UDP - this does actually needs a established connection to transsfer data becauuse this just sends out data and does not reseavs the data from any one it can afford to do that and that makes it a lot more faster than usual 
protocols: 
--------------------
TCP: HTTP, HTTPS, tailgate
UDP: DNS, RIP, VOIP 
packet order: 
--------------------
TCP: tcp has to maintain a packet order and to do that evry and each one of the oacjets actually gets assgned a indivisual nuumber to them and then they get sent over to the reciever 
UDP: this does not do any of that it just force sends all the packets that it needs to send to therecever and then the work is doen for it 
transmission speed:
--------------------
TCP: this has a morderate transmission speed because all the packages are actully getting assigned and then then sent over and in thid delivery process if anything gets damages or corrupted or anything that dupplicats or gets deleted then the files that are getting sent willl not just have a failure they will be picked out and will have to be resent by the main syetem to the reciever 
UDP: does not do none of that so the transmission speed is really fuckingn high but then the problem is that there is no guarantee of the transfer will actually happen 
reliability: 
--------------------
TCP: this is actally reliable from the accuracy perspective becsue we know that this connection might be aa little slow than UDP but even if there is a problem while sending over the packages it can fix that itself and send it with assurance 
UDP: from thr speed perspective it is reliable but there is not really a sequence virsitility so any of the sequence edits that have to be done in this files needs to bee done in the appplication layer before thee files are actually sent 
load: 
--------------------
TCP: the load is actually morderate because the a lot of files are not getting sent at a time rather they are gettiing sent in a synchronioyys manner
UDP:  on the other hand UDP network load is really really high because the damn filesjust gets sent all at a time 
data flow control: 
--------------------
TCP: Moderate network load. TCP requires three packets to set up a socket connection, before any user data can be sent. TCP handles reliability and congestion control. Because a TCP connection is bidirectional (can send and receive messages), each direction will have to be terminated independently.
UDP: sends everything at one time and does not avoid any kind of congession at any cost and just like i said before to avoind congession and make sure that while transfer the network ddo not face any issues we need to arrange them while being in ther application layer
troubleshooting capallilities: 
--------------------
TCP: has, because it can see what are the files that got damaged in the datastream and then send those files again over to reseaver from the original storage 
UDP: nada
handshake: 
--------------------
TCP: SYN, SYN-ACK, ACK handshake 
UDP: no handhake 


