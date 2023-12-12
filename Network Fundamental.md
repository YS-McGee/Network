# Network Fundamental


## OSI Model

### Application L7
Application layer is the layer in which protocols and rules are in place to determine **how the user should interact with data sent or received**.

### Presentation L6
This layer acts as a **translator** for data to and from the application layer (layer 7). 

The receiving computer will also understand data sent to a computer in one format destined for in another format. For example, when you send an email, the other user may have another email client to you, but the contents of the email will still need to display the same.

Security features such as data encryption (like HTTPS when visiting a secure site) occur at this layer.

### Session L5
Session layer will divide the data sent into smaller chunks of data and begin to send these chunks **(packets)** one at a time.

### Transport L4
* TCP
* UDP

Layer 4 of the OSI model plays a vital part in transmitting data across a network.

### Network L3
Network layer is where the magic of routing & re-assembly of data takes place (from these small chunks to the larger chunk).

Briefly, these protocols include OSPF (Open Shortest Path First) and RIP (Routing Information Protocol). The factors that decide what route is taken is decided by the following:

* What path is the shortest? I.e. has the least amount of devices that the packet needs to travel across.
* What path is the most reliable? I.e. have packets been lost on that path before?
* Which path has the faster physical connection? I.e. is one path using a copper connection (slower) or a fibre (considerably faster)?

### Data Link L2
The data link layer focuses on the **physical addressing** of the transmission. It receives a packet from the network layer (including the IP address for the remote computer) and adds in the physical MAC (Media Access Control) address of the receiving endpoint. Inside every network-enabled computer is a **Network Interface Card (NIC)** which comes with a unique MAC address to identify it.

### Physical L1
Put simply, this layer references the physical components of the hardware used in networking and is the lowest layer that you will find. Devices use electrical signals to transfer data between each other in a **binary numbering system (1's and 0's)**.

### Packets & Frames
packet: data that have IP info.
frame: dta that does not have IP info.

## Port Forwarding
Similar to NAT

## VPN 
VPN Technology
* PPP:
    Used by PPTP to allow for authentication and provide encryption of data.
* PPTP (Point-to-Point Tunneling Protocol):
    Easy to set up, but weaker than IPSec
* IPSec:
    Encrypts data using the existing IP framework
    
## VLAN
Allows specific devices within a network to be virtually split up. 
![image](https://hackmd.io/_uploads/BJEOR4BIa.jpg)

