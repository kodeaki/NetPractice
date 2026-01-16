*This project has been created as part of the 42 curriculum by kodeaki.*

# NetPractice

## Description
NetPractice is a project that aims to introduce the basics of networking through 10 increasingly difficult interactive levels. The project offers practical experience in network administration with non-functional network diagrams which need troubleshooting.

## Instructions
1. Download and extract net_practice.1.7.tgz
2. Run index.html in your application of choice.
3. 
    - Choose the "Training" interface for going up the levels starting from 1.
    - Choose the "Evaluation" interface for 3 random levels between 7-10 to practice on.
4. In each level, after completing it, press the "Get my config" to download a .json file which has your network configuration in it (aka what you have typed into the fields).
5. Submission requirements for the project are completing all 10 levels, submitting said levels' working configs into the given school repository's root along with this README.md and completing the peer evaluations.

## Resources
### Fundamental concepts to understand regarding this project (summarized)

  -  Data packets
      -  Sending large files over a network is quite unoptimized so data gets chopped up into smaller parts called data packets. Here's an example of what could happen if this wasn't done. If a network connection between a place A and place B is preoccupied with a transfer of a 10GB video file, a short email wouldn't be able to use that connection. It would either have to wait for the file transfer to finish, or take another less efficient route ie. A -> F -> B. But if data is divided into small packets, the email will slip right through the efficient A -> B connection.
  -  IP
      -  IP or Internet Protocol is a set of rules regarding how data is sent and received over the internet. It uses "IP addresses" as the destination point for the data being sent. In a similar way to real life addresses, like how a letter can be sent from anywhere with a unique address, and that letter will move onward from post office to post office, the data packets will go from router to router before ending up at the specified IP address. Except instead of roads the data travels between cables or the air (radiowave magic).
  -  TCP
      -  TCP or Transmission Control Protocol is a layer added on top of IP to ensure reliability. IP in itself is fast but basic. It only sends data packets to a specified IP address. It has no knowledge of whether the packet actually reached it's destination. That's where TCP comes in.
