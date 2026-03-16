# Project Aim

To develop a **multi-client chat application using Socket Programming in C on Windows** using the Winsock library.

---

# Project Description

This project is a **multi-client chat application** implemented using **C programming language and Winsock2 library on Windows**.

The system allows multiple users to connect to a server and communicate in real time.

### Features

* Multiple client connections
* Group messaging
* Private messaging using `@username`
* User authentication (username & password)
* Server-side chat logging
* Real-time communication between clients

---

# Tools & Technologies Used

| Component            | Technology  |
| -------------------- | ----------- |
| Programming Language | C           |
| Platform             | Windows     |
| Networking Library   | Winsock2    |
| IDE                  | VS Code     |
| Compiler             | GCC (MinGW) |

---

# Project Structure

```
chat-application/
│
├── chat_server.c
├── chat_client.c
├── chatlog.txt
└── README.md
```

---

# Installation Requirements

Install **MinGW (GCC Compiler)** if not already installed.

Check installation using:

```bash
gcc --version
```

---

# How to Compile & Run

### Step 1: Open Terminal

Open **Command Prompt / Terminal** in the folder where:

```
chat_server.c
chat_client.c
```

are located.

---

### Step 2: Compile the Server

```bash
gcc -o chat_server.exe chat_server.c -lws2_32
```

---

### Step 3: Compile the Client

```bash
gcc -o chat_client.exe chat_client.c -lws2_32
```

---

### Step 4: Run the Server

```bash
chat_server.exe
```

---

### Step 5: Run Clients

Open **one or multiple terminals** and run:

```bash
chat_client.exe
```

Multiple clients can connect to the server simultaneously.

---

# Example Chat Flow

1. Client starts the application
2. User enters **username and password**
3. Server **authenticates the user**
4. Users can send:

### Public Message

```
Hello everyone!
```

### Private Message

```
@Roshni Hello Roshni
```

Only the specified user will receive the private message.

---

# Chat Logging

All chat messages are saved on the server side in:

```
chatlog.txt
```

The log file contains **messages with timestamps**.

---

# Output

### Private & Public Chat Example

Shows communication between multiple users including public and private messages.

### Chat Log Example

Server stores all chat messages inside `chatlog.txt`.

---

# Project Status

**Completed & Working**

---


