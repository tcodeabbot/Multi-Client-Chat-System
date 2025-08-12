# Multi-Client Chat System (C)

## 📌 Overview
This is a multi-threaded TCP chat application written in C.  
It allows multiple clients to connect to a central server and exchange messages in real time.  
The project demonstrates **POSIX sockets**, **multithreading with pthreads**, and **mutex synchronization** for thread-safe operations.

## 🚀 Features
- Real-time messaging between multiple clients.
- Supports up to 10 concurrent users.
- Handles client join/leave notifications.
- Thread-safe client management using mutex locks.
- Gracefully handles unexpected disconnections.

## 🛠 Technologies Used
- **Language**: C
- **Networking**: POSIX Sockets
- **Concurrency**: POSIX Threads (pthreads)
- **Compiler**: GCC

## ⚙️ Installation & Usage

### 1️⃣ Compile the Server
```
gcc server.c -o server -pthread
```
### 2️⃣ Compile the Client
```
gcc client.c -o client -pthread
```
3️⃣ Run the Server
```
./server
```
4️⃣ Run Clients (in separate terminals)
```
./client
```
#### Note: The server must be running before clients can connect.

🧪 Testing
Start the server, then connect multiple clients.

Send messages from one client and see them appear in others.

Close a client to test disconnection handling.

Try sending empty messages or connecting more than 10 clients.

📜 License
This project is open-source and available under the MIT License.
