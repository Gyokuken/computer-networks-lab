# Computer Networks Laboratory

This repository contains a set of networking experiments demonstrating socket programming, client–server architectures, and multithreading using **C** and **Python**. Each lab is focused on implementing core networking concepts in a practical, hands-on manner.

---

## Lab 1: Basic Client–Server Communication
**Objective:** Implement a simple TCP-based client–server setup.  
**Languages:** C, Python

**Topics Covered**
- Socket creation and binding  
- Listening for and accepting connections  
- Message transmission between client and server  
- Handling basic requests  

---

## Lab 2: Multithreaded Server and Client Simulation
**Objective:** Build a multithreaded server capable of handling multiple clients concurrently.  
**Languages:** C, Python

**Topics Covered**
- Creating and managing threads  
- Handling multiple clients simultaneously  
- Simulating multiple clients on a single system  
- Synchronizing shared data  

---

## Lab 3: Simple Web Server in C
**Objective:** Implement a minimal web server that responds to HTTP GET requests and serves an `index.html` file.

**Topics Covered**
- TCP socket creation and binding (typically port 8080)  
- Managing browser connections  
- Parsing HTTP GET request headers  
- Responding with `HTTP/1.1 200 OK` and HTML content  
- Inspecting communication using Wireshark  

### Implementation Steps
1. Create an `index.html` file to be served.  
2. Write `webserver.c` to accept connections and serve the HTML content.  
3. Compile the program:
   ```bash
   gcc webserver.c -o webserver

4. Run the server:

./webserver


5. Open the browser and visit:
http://localhost:8080


6. Inspect packets using Wireshark to observe:

TCP three-way handshake

HTTP GET request from the browser

HTTP response carrying the HTML file





---

Getting Started

Requirements

C

GCC compiler

pthread library


Python

Python 3.x (standard socket module)



---

Compilation and Execution (C Programs)

# Compile and run the multithreaded server
gcc server.c -o server -pthread
./server

# Compile and run the client(s)
gcc client.c -o client
./client 1
./client 2


---

Features

Multi-client handling through multithreading

Simulation of multiple clients on the same machine

Demonstrations written in both C and Python

Minimal HTTP web server implementation using raw sockets

Clear and modular lab structure for easy navigation
