*This project has been created as part of the 42 curriculum by kodeaki.*

# NetPractice

## Description
NetPractice is a project that aims to introduce the basics of networking through 10 increasingly difficult interactive levels. The levels are made of non-functional network diagrams which the user needs to configue back into working order. The project offers valuable practical experience in network administration and troubleshooting.

## Instructions
1. Download and extract net_practice.1.7.tgz
2. Run index.html in a web browser of your choosing.
3. 
    - Choose the "Training" interface for going up the levels starting from level 1.
    - Choose the "Evaluation" interface for 3 random levels between 7-10 to practice on.
4. In each level, after completing it, press the "Get my config" to download a .json file which has your network configuration in it (aka what you have typed into the fields).
5. Submission requirements for the project are completing all 10 levels, submitting said levels' working configs into the given school repository's root along with this README.md and completing the peer evaluations.

## Resources
### Fundamental concepts to understand regarding this project (summarized)

  - **Data packets**  
  
    Sending large files over a network is quite unoptimized so data gets chopped up into smaller parts called data packets. Here's an example of what could happen if this wasn't done: If a network connection between a place A and place B is preoccupied with a transfer of a 10GB video file, a short email wouldn't be able to use that connection. It would either have to wait for the file transfer to finish, or take another less efficient route ie. A -> F -> B. But if data is divided into small packets, the email will slip right through the efficient A -> B connection.

  -  **Routers**
  
        Routers are devices that route data packets between devices, networks, internet, etc. Most routers - and the ones people are most familiar with - forward data between LANs (Local Area Networks) and WANs (Wide Area Networks. In simple terms LANs are your home or office networks that usually have one router that devices are connected to. WANs are networks that connect multiple LANs together

  -  **Switches**  
  
        Switches are network devices that are used to split networks into subnetworks aka subnets or LAN segments. They use MAC addresses to filter and forward packets between subnets. Switches, among other things, can transfer data to a specific address instead of the whole network which allows efficient bandwith use.

  -  **IP**  
  
        IP or Internet Protocol is a set of rules regarding how data is sent and received over the internet. It uses "IP addresses" as the destination point for the data being sent. In a similar way to real life addresses, like how a letter can be sent from anywhere with a unique address, and that letter will move onward from post office to post office, the data packets will go from router to router before ending up at the specified IP address. Except instead of roads the data travels between cables or the air (radiowave magic).

  -  **TCP**  
  
        TCP or Transmission Control Protocol is a layer added on top of IP to ensure reliability. IP in itself is fast but basic. It only sends data packets to a specified IP address. It has no knowledge of whether the packet actually reached it's destination. That's where TCP comes in.

  -  **Subnet masks**  
  
        32-bit masks that separate an IP address into network bits and host bits. Network bits are used to identify the network and host bits are used to identify a device on that network.

  -  **Default Gateway**  
        Default gateway is a device that allows another device to communicate with devices on other networks, usually a router. Devices on the same network can communicate with each other directly without going through a gateway but to talk to devices on other networks they need to send the data through a gateway. A default gateway is the path that data takes when the destination IP doesn't match any route specifications. Example: 2 devices in a network with IP addresses 192.168.0.2 and 192.168.0.3 and a router with the IP of 192.168.0.1. If device 192.168.0.2 sends a packet with an IP of 192.0.2.1 assigned to it, 192.168.0.3 would ignore the package but the default gateway aka the router 192.168.0.1 would forward that packet.

  -  **OSI layers**
  
        The OSI model is a framework that describes network communications protocols. Developed by the International Organization for Standardization (ISO), it's purpose is to standardize the ways in which systems communicate with each other. In the model communication systems are divided into seven abstraction layers: Application, Presentation, Session, Transport, Network, Data link, Physical. Starting from the top with Application being the interface that the end user sees and/or communicates with, all the way down to the physical layer which describes the physical properties of electrical connectors, frequencies to transmit on, etc.


## Use of AI
AI was used as a search assistant when studying the mentioned topics but was not used as a single source of information. Remember that AI is not always a reliable tool and can give false information. All the information listed in this README was also confirmed from trusted and reliable sources.
