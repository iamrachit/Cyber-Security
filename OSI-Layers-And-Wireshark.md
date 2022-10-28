# OSI Layer

## Application Layer = User Interaction 

## Presentation Layer = Data Format 

live session / webinar 

study material 

whatsapp 

1. formating of data - Image/video/gifs/audion

2. Encoding and Deconding - base64
 
4. Encryption and Decryption - hello - simple text stored in encrypted 

## Session Layer = social media - logout - gamil - session - time sync

## Transport Layer = Direction 

live session => UDP - Unit Datagram Protocol 

TCP => Transmission Control Protocol 

**Which communication is faster UDP vs TCP ?**

UDP - faster | Because we are nto waiting for confirmation.

## Network Layer
 
Internet layer (wifi connection)

Logical Address -  IP address but its not the permanent address 

Data Link - Permanent Address - Mac address - Media Access Control 

## Physical Layer - Wired Connection with the help of electricity 

# Wireshark

It is a Network Protocol Analyzer which capture 7 layers.

## How does it do ?

![image](https://user-images.githubusercontent.com/60937657/198268507-6f843dce-ef26-4b98-bc7f-3903c7377578.png)

It monitor all the system connected to network through wifi or routers for example its like a security guard.

Wireshark file extension is .pcap or .pcapng

## Drawback of wireshark 

It can not decrypt the data /msg which we are sending from one system to another or in network.

# Type of data send in different layer and type of data format

Application - Data

Presentation - Image/Audio/Video

Session - Time Format 

Transport - Segments

Network - Packets 

Data link - Frames

Physical - Bits/Bytes Formats

**Type of Data Format**

Hex Decimal Format - 0123456789 ABCDEF = 16

Decimal Number = 0123456789 = 10

Octal Number = 01234567 = 8

Binary Number = 0 and 1 = 2 

## TCP 

It include Three Way Handshake process in which firstly the client sends a pur SUN segment indicating it wants a connection and secondly the server responds with SYN-ACK segmennt which means it acknowledged the request and is sending its onw SYN number for the client to acknowledge. 

![image](https://user-images.githubusercontent.com/60937657/198494363-9f503f4e-49d9-47e4-8c5a-e6421ee3ef28.png)

![image](https://user-images.githubusercontent.com/60937657/198495072-7e1fcc0d-0376-45d3-abfb-187ab8afbe8b.png)

**6 Type of flags in TCP header**

1. ACK - Acknowledgment -  We are getting confirm 
2. SYN - Synchronization - it will just initate 
3. RST - Rest - communication go in rest phase 
4. FIN - Finish -  we just finish communication 
5. URG - Urgent - urgent 
6. PSH - Push - when data/network formwarding 




