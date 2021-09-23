{
  "title": "TCP vs UDP",
  "date": "2021-08-31T10:19:39-05:00",
  "draft": false,
  "author": "Said Neder",
  "tags": ["Networking"]
}

# TCP, UDP, and the three-way handshake

Both are layer 4 of the OSI model, that is transport, so this protocols covers the transport of packets to the application.

## TCP
TCP = Transmission control protocol

Protocol for sending and receiving data

The communication between two computers need to be "good" and reliable, to guarantee that the data is received correctly, like a webpage or downloading a file, this protocol is used to guarantee that all the data is received and in order.

TCP is a connection-oriented protocol, which basically means that it must first acknowledge a session between the two computers that are going to communicate, so the two computers verify a connection before any communication takes place.

**First step:**
The first computer will send a SYN, that is message.

**Second step**
Then the other computer will send a SYN ACK, that is a message acknowledging the SYN message.

**Third step:**
Then the first computer will send a ACK, that is acknowledging the the SYN ACK so now they confirmed that they have a stable connection where data can be delivered.

And that is known as the ***Three way handshake***

This protocol guarantees the delivery of the data so if a packet is missing it will re send it and let the other computer know.

## UDP
UDP = User datagram protocol

Protocol for sending and receiving data

UDP is a connectionless oriented protocol, and it does not establish a session and because of that it does not guarantee data delivery, is just sends all the packets, it doesn't matter if it is received at the end or not.

That's why is known as a "fire-and-forget" protocol, but thanks to not guaranteeing data delivery, is much faster than TCP, UDP is used in livestreams, where you want a fast connection that gives you the live moment of your soccer match for example, you don't want to be 10 seconds delayed for a pixel that it wasn't sent as would be in TCP.
