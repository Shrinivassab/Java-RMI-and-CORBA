Implementing distributed system with java RMI and CORBA: 
	• RMI (Remote Method Invocation) - using java programming language and development environment  , we can create object oriented programming in which objects on different computer can interact in an distributed network.
	• Is  known as RPC with a ability to pass one or more request.
	• The object contain information that have the ability to change the service that is performed in the remote computer. EXAMPLE :  User at remote computer fills the expense account , the java program interacting with the user can communicate using RMI with java in another computer that always had the latest policy about expense reporting. In reply, that program would send back an object and associated method information that would enable the remote computer program screen the user's expense account data in a way that contain latest policy. The user and the company both would save time by catching mistake early . Whenever company policy changed, it would require a change to a program in only one computer.
	• CORBA:
		○ Which is a model component
		○ Common Object Request Broker Architecture. " is an architecture and specifies for creating, distributing and managing distributed program objects  in a network". It allows program at different location and developed by different vendor to communicate in a network through interface broker .
		○ In CORBA most important concept is ORB (Object Request Broker)- > Support in a network of clients and servers on different computers means that a client program can request service form a program or whatever the interface in the server program looks like.
	• WHAT I IMPLEMENTED :
		○ Developed basic internet chat system using java RMI.  
		○ My system will enable two users to exchange text messages over the internet using simple graphical interface. 
			§ We were told to use either client server architecture or peer to peer architecture.
			§ I used Peer to Peer architecture because I want each workstation to have equivalent responsibilities which is totally different from client server architecture in which some computers are dedicated to server other. Which is simpler, and it won't handle heavy load. 
			§ If I am going to handle heavy load I will go with client server architecture.
		○ My program contain
			§ Basic user interface with 2 text areas.
			§ The first text area used to enter text and sent to remote client.
			§ I am free to use any transmission strategy - which means how I can sent message "I made it in such a way that it can handle one text at a time" and clear the entry area after each transmission.
			§ The second text area will display text received form the remote client. 
			§ The client application will enable user to identify the address of the remote chat participant.
		○ Then I implemented same thing with CORBA:
			§ Implemented in my LAB where I can get the java SDK has CORBA ORB.
