# http-server
1. Introduction
The HTTP Server is a basic implementation of a web server that handles client requests over the HTTP protocol. It is designed to demonstrate core networking concepts such as socket communication, request parsing, and response generation.

2. Objectives
Understand how HTTP protocol works
Learn socket programming fundamentals
Implement a basic client-server architecture
Serve static web content

3. System Architecture

The system follows a client-server model:

Client: Web browser sends HTTP requests
Server: Processes requests and returns responses
File System: Stores static files to be served

Workflow:

Client sends request
Server receives request via socket
Request is parsed
File is retrieved
Response is sent back

4. Technologies Used
Programming Language: Python / Node.js / Java
Networking: Socket Programming
Protocol: HTTP/1.1

5. Module Description
5.1 Server Initialization
Creates a socket
Binds to a port (e.g., 8080)
Listens for incoming connections
5.2 Request Handling
Accepts client connection
Reads HTTP request
Extracts method, path, headers
5.3 File Handling
Maps requested URL to local file
Reads file content
Handles missing files (404 error)
5.4 Response Generation
Constructs HTTP response
Adds status line (200 OK, 404 Not Found)
Sends headers and body
