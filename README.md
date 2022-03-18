Version-2 Using the serialize interface for performing server, packet and client sync Used the ObjectInput and ObjectOutput streams of the sockets for transferring information to and fro between server, client and client , client

List of Files:
In addition to this README file, the Project submission consists of three files:

Client.java : Connects to a server, enters a chat room of its choice in order to exchange messages with other clients.
Server.java : Accepts connections from clients, puts a client in the requested chat room
Packet.java : Abstract implementation of generic packets
Instructions for Compiling the program:
Compile the Client: javac Client.java
Compile the Server: javac Server.java
Compile the ChatRoom: javac Packet.java
Instructions for Running the Program:
Start the server: java Server
The server GUI window will open and then ask the user to connect to the
Start the client: java Client (Type this command in a different xterm/terminal). For more clients, open several xterms and type this command.
Enter the IP address of the server: a) if client and server are on the same system, then enter "localhost" and click "Ok". b) else, enter the IP address of the server (e.g., "10.0.0.5") and click "Ok".
Enter a unique client name (e.g., "Parth") and click "Connect to Server".
The list of rooms is being displayed in the client window and the client can enter/create a room by using @join / @create
The client can leave a room using @leave
The list of users is displayed on the client GUI window as well as on the server GUI window
Host can remove any client using the @remove
Users can send private messages to each other using the @user command
