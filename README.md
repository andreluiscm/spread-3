File Service
============
This project is a Simple distributed file service, implemented during the Distributed Systems Class.
The project was developed using the Spread Toolkit and provides a Server, Slave and Client interfaces.
Using the Client interface you are able to create (choosing the number of copies), delete, read and write files.

Technologies
-----
* Spread Toolkit - version 4.4 (http://spread.org/)

Building
-----
To compile the project, from inside the source folder (src), run the command below:
```
javac -cp .:../lib/* Server.java Client.java Slave.java
```
The Server, Slave and Client executables will be generated.

Usage
-----
0. Run the Spread daemon.
1. This step forward, will be assumed that you will be running the codes shown here from inside the source folder (src). Run a Server passing a flag "-s" followed by its value containing the "server name" followed by an underline "_" and a number id "x" of your choice, and a flag "-r" followed by its value containing the priority of the Server, like the command below:
```
java -cp .:../lib/./* Server -s server_1 -r 1
```

2. Run a Slave passing a flag "-s" followed by its value containing the "slave name" followed by an underline "_" and a number id "x" of your choice, like the command below:
```
java -cp .:../lib/./* Slave -s slave_1
```

3. Run a Client passing a flag "-c" followed by its value containing the "client name" followed by an underline "_" and a number id "x" of your choice, like the command below:
```
java -cp .:../lib/./* Client -c client_1
```
4. Follow the menu shown in the Client interface.

Notes
-----
0. You are able to instantiate as many Servers, Slaves and Clients as you want to.
1. Some bugs may be found and, if found, feel free to mail to my e-mail located at my profile page.
