This project is a Java-based remote administration experiment designed to explore network communication, system control, and firewall behavior. The system uses Java, SQL, and a peer-to-peer communication approach to allow a server application to send commands to connected client machines through a database-based messaging mechanism.

The project consists of three main components. The Server application is used to manage connected clients and send commands. The Client application runs on the target machine and listens for commands by monitoring changes in the SQL database. The Config application is used to configure and connect the server and client components.

Communication between the server and client is implemented through an SQL database. The client periodically checks the database for command updates. When a change is detected, the client processes the command and returns the requested information back through the database. This approach was implemented to study firewall behavior where outgoing connections are generally allowed while incoming connections are restricted.

The system supports several core features. The server can display all connected client machines, browse files and directories on the client system, and download files from the client computer.

The project requires a running database server in order to function. The database acts as the communication layer between the server and client applications.
