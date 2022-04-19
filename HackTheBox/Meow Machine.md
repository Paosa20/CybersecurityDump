Initial machine in HackTheBox

Meow Machine


 What does the acronym VM stand for? 
 - Virtual Machine

What tool do we use to interact with the operating system in order to start our VPN connection? 
- Terminal

What service do we use to form our VPN connection? 
- openvpn

What is the abreviated name for a tunnel interface in the output of your VPN boot-up sequence output? 
- tun

What tool do we use to test our connection to the target? 
- ping (try it out ping [IP])

 What is the name of the tool we use to scan the target's ports? 
- nmap (Basic nmap scan= nmap [IP])

Now we can try it with our target IP address and it tell us that, Port 23 TCP is open. Write down this as it is very useful for later !
![[Pasted image 20220418185253.png]]


What service do we identify on port 23/tcp during our scans? 
- Telnet

What username ultimately works with the remote management login prompt for the target? 
- root

Submit root flag 
 1. Remember the scan we made? when doing nmap [IP] as a result it said that that port 23 is open, which means we can exploit this. Now how do we connect via telnet? Add the next command on youir terminal : telnet [IP] 23 (telnet [IP addres we want to connect to] [Port])
 2. It asks for the Meow login, we can try root as mentioned before and lucky for us it worked!
  ![[Pasted image 20220418185855.png]]
 3. Now that we have access to the machine we can use the next command "ls" to check what we may have acces to
![[Pasted image 20220418185925.png]]

4. We can see an archive called "flag.txt" and that is our last objective, use the next command to get the flag "cat flag.txt"

Congrats you got yout first flag! Keep it up!