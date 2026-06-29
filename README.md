# Java Chat Server

A real-time client-server chat application built with **Java**, using **Sockets** for network communication and **Java Swing** for the GUI. Supports multiple clients connecting simultaneously through a central server.

## Features

- Real-time two-way messaging between server and clients
- Multi-client support — multiple users can connect simultaneously
- Java Swing GUI for both server and client sides
- Server connection and message logs for monitoring
- Graceful handling of client disconnects

## Tech Stack

| Category | Tools |
|---|---|
| Language | Java |
| Networking | Java Sockets (TCP) |
| GUI | Java Swing |
| Architecture | Client-Server |

## Project Structure

```
chatserver/
├── ServerEnd.java    # Server-side logic and GUI
└── ClientEnd.java    # Client-side logic and GUI
```

## Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/Shrutiraj26/chatserver.git
cd chatserver
```

**2. Compile both files**
```bash
javac ServerEnd.java
javac ClientEnd.java
```

**3. Start the Server**
```bash
java ServerEnd
```

**4. Start a Client (in a new terminal)**
```bash
java ClientEnd
```

You can open multiple terminals and run `java ClientEnd` in each to simulate multiple users chatting simultaneously.

## How It Works

1. The server starts and listens on a port for incoming connections
2. Each client connects to the server via TCP socket
3. Messages sent by a client are received by the server and broadcast to all connected clients
4. The server logs all connections, disconnections, and messages in real time
5. When a client disconnects, the server handles it gracefully without crashing

## Concepts Demonstrated

- Java Socket Programming (TCP)
- Multi-threading for handling concurrent clients
- Event-driven GUI with Java Swing
- Client-Server architecture
