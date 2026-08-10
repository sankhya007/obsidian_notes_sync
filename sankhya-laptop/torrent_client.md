so this is the project that i am just trying to see if i can actually make a system that can beat the existing torrent clients in the market in any kind of ways
just trying to see if a torrent client can have a quirk of sort that will amke it different than the existing onces 

for now on the main task that i want to do is : 
1. make the most basic torrennt client possible and make it run un the terminal and open source it and actually make it in a sort that i actually use it rather(should not be a hasle to use)
2. its okay if it does not have an interface an termminal interface in all that i ask for because that is the only crutial thing that i need to understand of the things are actually working or no 
3. DO NOT make a educational malware like last time, no silumation no nothing bulllshit. only write what wee need to have 
4. understand evrything that we write and have in the code, i am make this not just to increase the aura of my resume but also to have a generational run on the project spree that i am in 

chapters : 
1. [[prerequisits]]
2. [[the_.torrent_file]]
3. [[tracker_comunication]]
4. [[peer_wire_protocol]]
5. [[piece_management]]

flow of the main torrent file : 
parse .torrent file -> contact tracker -> get peer list -> TCP connect to peers -> handshake -> unchoke exchange -> request blocks -> verify pieces -> write to disk 

[[basic understanding]]
