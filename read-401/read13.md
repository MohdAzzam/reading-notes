# Message Queues

A Queues of messages sent between applicatios includes a sequence of work object wating to processe 

A message queue provides an asynchronous communications protocol, which is a system that puts a message onto a message queue and does not require an immediate response to continuing processing. Email is probably the best example of asynchronous communication. When an email is sent, the sender continues to process other things without needing an immediate response from the receiver. This way of handling messages decouples the producer from the consumer so that they do not need to interact with the message queue at the same time.

1. once the initial handshake has taken place and the connection is established, the client and server can both communicate with each other freely
2.  
3.  The event gets passed to the server through websockets. Its a tcp connection from the browser to the server. The connection is full duplex meaning the server can send real time data to the client and vise versa.
4.  it can cause a website to freeze and become unstable 
5.  handel this or prevent it 



### Rooms 

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients:
rooms are a server-only 

