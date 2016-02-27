# Socket-Programming

PROJECT DESCRIPTION

• The program can run on any available port of the system.
• Multiple requests can be handled by the server at the same time. Client requests are handled in separate threads.
• If the file exists on the server, the server responds with "HTTP/1.1 200 OK” along with the contents of the file. If the file   is not found, server responds with a "HTTP/1.0 404 Not Found” message.
• Messages exchanged between the server and the client are written into a log file.

PREREQUISITES

• JDK 1.8
• Apache or Xampp Server (Any version)

PROGRAM EXECUTION INSTRUCTIONS

• Install JDK 1.8.
• Open CMD in windows and navigate to the path where the zipped file has been extracted.
• Compile the three java files using the following commands:
javac WebServer.java
javac WebClient.java
javac HttpRequestGet.java
• Run the server code(eg: ‘java WebServer 5000’). The port number should be given as an argument. The server starts waiting for a client.
• Open a new terminal window (CMD in windows) and navigate to the project directory.
• Compile all the three Java Files with the commands mentioned above.
• Run the Client program “WebClient.java”. The program takes the URL as an argument. Eg: java WebClient       http://localhost:5000/gameofthrones.html . The contents of the file are
displayed on the terminal and displays the RTT time.

ERROR HANDLING
• Entering an incorrect url on the Client Side
• File not found
• The log details are stored in log.txt file

CLIENT AND SERVER CHARACTERISTICS

• Client requests for a file given the IP Address and port number of the server.
• Client establishes a connection with the server using sockets.
• If the connection is successful, client gets the “HTTP/1.1 200 OK” message along with the content of the file.
• If the connection fails, the client gets the “HTTP/1.0 404 Not Found” error message.
• All Server side requests are stored in the log file.



REFERENCES
https://docs.oracle.com
http://tutorials.jenkov.com/java-multithreaded-servers/multithreaded-server.html
http://www.javatpoint.com/socket-programming
http://www.oracle.com/technetwork/java/socket-140484.html
http://www.tutorialspoint.com/javaexamples/net_multisoc.htm
