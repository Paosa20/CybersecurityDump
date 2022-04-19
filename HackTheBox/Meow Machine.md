# Initial machine in HackTheBox

## Meow Machine


 #### What does the acronym VM stand for? 
 - Virtual Machine

### What tool do we use to interact with the operating system in order to start our VPN connection? 
- Terminal

### What service do we use to form our VPN connection? 
- openvpn

### What is the abreviated name for a tunnel interface in the output of your VPN boot-up sequence output? 
- tun

### What tool do we use to test our connection to the target? 
- ping (try it out ping [IP])

 ### What is the name of the tool we use to scan the target's ports? 
- nmap (Basic nmap scan= nmap [IP])

![image](https://user-images.githubusercontent.com/55120196/163901557-0e52640f-81fe-49cc-b8b6-666a4cf4a337.png)


Now we can try it with our target IP address and it tell us that, Port 23 TCP is open. Write down this as it is very useful for later !

### What service do we identify on port 23/tcp during our scans? 
- Telnet

### What username ultimately works with the remote management login prompt for the target? 
- root

### Submit root flag 
 1. Remember the scan we made? when doing nmap [IP] as a result it said that that port 23 is open, which means we can exploit this. Now how do we connect via telnet? Add the next command on your terminal : telnet [IP] 23 (telnet [IP addres we want to connect to] [Port])
 
 ![image](https://user-images.githubusercontent.com/55120196/163901675-a70decf6-dfe4-4471-9e89-7d422aa3279f.png)

 2. It asks for the Meow login, we can try root as mentioned before and lucky for us it worked!
 
 ![image](https://user-images.githubusercontent.com/55120196/163901640-ddc446d8-e713-4dc9-a651-93c67e7bb36b.png)

 3. Now that we have access to the machine we can use the next command "ls" to check what we may have acces to

 4. We can see an archive called "flag.txt" and that is our last objective, use the next command to get the flag "cat flag.txt"

![image](https://user-images.githubusercontent.com/55120196/163901731-f00f2a47-2c85-462c-8aac-bdff9221ac26.png)

## Congrats you got your first flag! Keep it up! 🐱
