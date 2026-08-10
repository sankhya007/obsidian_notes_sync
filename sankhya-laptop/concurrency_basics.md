when downloading a torrent file the client connects to a lot of peers simultaniously to request and send file pieces, if the client proceeds these connections one by one synchroniously a slow peer would freeze the entire download. 

to keep everything mmoving at once we need need concurrency, and there are two methods to that concurrency 

multithreading(dedicated workers)
----------
here we are goign tohave a dedicated worker or a thread for every peer the client of going to connect to 

-  working principal - thread A taks to peer A and thread B is gonna talk to peer B they all run at the same time 
-  trade off - simple to write and efficient but it is really memory intensive it is managing hundreads not thousands of active threada and pulling data all together from there, this actually slows down the system by a lot and that maked the whole thing un usable(the main cause of that is context overhead switching)

asynnc I/O & event loop(the singlle juggller)
----------
instead of many workers here the client is goign to assign one worker to do the job and they are going to run a continus loop 

-  working principal - the event loop is goign to ask the operating system that which peer has data ready to download of reall in that immediate moment and then it is going to download the data from that peer/ seeder and write that data to the disk and when done it moves on to te next one and keeps on writting to the disk
- ideal for torrents - ppeer connections spend most of their time waiting on the network and an event loop does not waste memory while waiting if only scts when a peer actually sends or requests data 

bottom line
==========
modern toorrents heavily rely on ASYNC I/O event loops because they can effortlessly manage thosands of simultanious peer connections using a fraction of the system memory if they were using multi-threading on that position instead. 