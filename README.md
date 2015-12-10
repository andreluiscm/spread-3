File Service
============
This project is a Simple distributed file service, implemented during the Distributed Systems Class.
The project was developed using the Spread Framework and provides a Server, Slave and Client interfaces.
Using the Client interface you are able to create (choosing the number of copies), delete, read and write files.

Technologies
-----
* Spread Toolkit - version 4.4 (http://spread.org/)

Building
-----
To compile the project, from the source folder (src), run the command below
```
javac -cp .:../lib/* Server.java Client.java Slave.java
```
The executables Server, Slaver and Client will be generated.

Usage
-----
0. Run the Spread daemon.
1. This step forward, will be assumed that you will be running the codes shown here from the source folder (src). Run a Server passing a flag "-s" followed by its value containing the "server name" followed by an underline "_" and a number id "x" of your choice, and a flag "-r" followed by its value containing the priority of the Server, like the command below. An election algorithm will automatically be called every time a new Server is started and joins the group.
  ```
  java -cp .:../lib/./* Server -s server_1 -r 1
