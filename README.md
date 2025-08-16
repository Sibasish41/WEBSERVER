WEBSERVER
A simple Java-based web server demonstrating three different threading models:
SingleThreaded
MultiThreaded
ThreadPool

Features:
```
📡 Single-Threaded Server: Handles client connections sequentially.
🔀 Multi-Threaded Server: Creates a new thread for every client connection using Java's Consumer functional interface.
⚡ Thread Pool Server: Uses ExecutorService to efficiently manage a fixed pool of threads for handling client requests.
```

Directory Structure:
```
WEBSERVER/
├── MultiThreaded/
│   ├── Server.java
│   └── Client.java
├── SingleThreaded/
│   ├── Server.java
│   └── Client.java
├── ThreadPool/
│   └── Server.java
└── .idea/

```

Getting Started->
Prerequisites:
Java JDK (8 or higher)
Command line/terminal access

Compilation
Navigate to the desired implementation folder and compile the .java files. For example:
```
cd MultiThreaded
javac Server.java Client.java
```
Running the Servers:
SingleThreaded Server:
1.Open a terminal in the SingleThreaded folder.
2.Run the server:
```
java Server
```
In another terminal, run the client:
```
java Client
```
MultiThreaded Server:
1.Open a terminal in the MultiThreaded folder.
2.Run the server:
```
java Server
```
In another terminal, run the client:
```
java Client
```
* The client spawns 100 concurrent threads to test multi-threading performance.
* 
ThreadPool Server
1.Open a terminal in the ThreadPool folder.
2.Run the server:
  ```
  java Server
  ```
  *This server uses a fixed-size thread pool for client connection handling.

Notes:
*All servers listen on port 8010 by default.
*You can adjust the port and thread counts in the source code as needed.
