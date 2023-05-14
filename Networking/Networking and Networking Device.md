# Computer Networking
Networking is a practice to exchange the data between nodes over a shared medium or operating system. It also involves management , maintenance and operationsof networks infrastructure software and policies.
Computer networking is everything that makes it possible for computers,servers and other devices to communicate.

Now we will be seeing various newtworking devices that are important to know how data flows in the network.

## Network Devices
### Host:
Host are any device that sends and receives traffic over the network
Client initiates the request and server responds to the request.
Here server is simply a computer with software installed that responds to specific request
![image](https://user-images.githubusercontent.com/76161912/236511527-0782caf9-44c5-4b27-8d96-8e5788c5b53b.png)

### IP Address:
1) IP address is identity of each host. it needs it to communicate on a network to send and receive packets.
2) The purpose of an IP address is to handle the connection between devices that send and receive information across a network
3) IP address is 32 bits
4) Each bit is just 0 and 1 . So IP address is just random 32 1's and 0's 
5) We break it into four octet and convert each octet into decimal number.
6) 1011  0110 1000  1101  0101  1101  1100  1010
7) When IP address are heirarchly assigned they are called Subnetting

### Network
1)A network is what transports the traffic between Hosts
2)Two hosts connected , we get a network.
3) Network can also be defined as logically grouping of host which require similar connectivity.
4) We can have network inside the network called Subnetworks or Subnets

#### What is Internet:
Network connect to other networks. Now there can be many networks and each network can not have its individual connection to one another. Hence they connect to a specific entity called Internet.
 INTERNET ->>> INTERconnected NETwork
 
 ### Repeater
 Now a network is established when two computers connect each other through a wire. The signal in the wire can decay as it travels. For this we need a repeater to amplify the signal.
 ![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/7cbcaacf-3b7c-4b6d-8eb1-c8aad3c6bb55)

##  A problem
Now lets discuss a problem. Imagine we have two hosts connected . What if we need more hosts . 4-5 hosts to be connected to each other. Now this is manageable at smaller scale but at large scale its not possible . We require a device to funnel the communication between different hosts then all hosts to be coming henceforth will be connected to this. This will reduce scalability issues. Hence we came up with Hub

### Hubs
![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/7e515895-08f0-4b44-bd21-0c61f2c465a1)

It is a multiport repeater. Many devices can be connected to it.
But here every device connected to this hub receives the signal for ex: a signal sent by Host A to Host B is received by other hosts a well .
Hence we use bridges

### Bridges
![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/d965e721-ac7f-4c2c-a34e-de79b1bd59a2)

It sits between two Hub connected hosts.
It have two Ports. Bridges learn which hosts are on which side. If Host A wants to send signal to host B , the signal goes to host B and bridge here is able to identify which host is on which side and signal remains in that HUB

### Switches
![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/e01f1f11-e00f-4fce-b6c9-ac1f7ae3f8e2)
Facilitate communication within network.
These are combination of HUBS and BRIDGES. 
These have multiple ports .
Learns which hosts are on each port

### Routers
![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/2c32cf22-9f51-4970-829b-36fbb25875f1)

Facilitate commuication between netwoks
Provide traffic control points between two different PC's of two different network(Security , Filtering , Redirecting.
Routers learn which network they are attached to know as routes which is stored in Routing table.
A Router has an IP address.
![image](https://github.com/VijayVPatil/DevopsWithVijay/assets/76161912/3cdda969-d87e-473a-afe2-a3643e2caae8)

This IP address is a gateway Local
Gateway: A host's way out of the network to connect to another hosts of another network.
