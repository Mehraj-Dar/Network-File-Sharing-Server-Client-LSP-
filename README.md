
-----

# 🧩 Network File Sharing Server & Client

**Author:** Mehraj Rustum  
**University:** Siksha ‘O’ Anusandhan University, Bhubaneswar  
**Department:** Computer Science & Engineering  
**Semester:** 5th (2025)  
**Project Type:** Capstone Project (LSP)

-----

## 🚀 Project Overview

This project implements a **Network File Sharing System** using **C++ and POSIX sockets**.
It enables a client and server to communicate over a **TCP connection** to **list, upload, and download files** securely.

The system is lightweight, efficient, and designed to demonstrate the core concepts of **socket programming**, **file handling**, and **data transmission** in computer networks.

-----

## 🎯 Objective

To develop a networked file-sharing application with a **server–client architecture**, supporting:

  * File listing on the server.
  * File transfer (upload and download).
  * Secure communication using simple encryption.
  * Real-time interaction between server and client.

-----

## ⚙️ Technologies Used

  * **Language:** C++
  * **Framework:** POSIX Sockets
  * **Operating System:** Linux / Ubuntu (or other POSIX-compliant OS)
  * **Tools:** GCC / G++ Compiler, Terminal

-----

## 📂 Project Structure

```
Network-File-Sharing/
│
├── server.cpp          # Server-side source code
├── client.cpp          # Client-side source code
│
├── server_files/       # Directory containing files shared by the server
│   ├── file1.txt
│   └── file2.pdf
│
├── client_downloads/   # Directory where client downloads are saved
│
└── README.md           # Project documentation
```

-----

## 💡 Features

  * 🧠 **Client–Server Communication:** Reliable two-way connection using TCP sockets.
  * 📁 **File Transfer:** Supports both upload (`PUT`) and download (`GET`) operations.
  * 📜 **File Listing:** Client can view all available files on the server.
  * 🔒 **Simple Authentication:** Server requires a password to grant access.
  * 🛡️ **Simple Encryption:** (Educational) All data is encrypted using a simple XOR cipher.
  * ⚡ **Lightweight Design:** Runs on minimal system resources.
  * 🧩 **Easy to Extend:** Simple architecture for students and beginners to build upon.

-----

## 🖥️ How to Run the Project

### 1\. Compile the Source Files

Open your terminal and compile both the server and client:

```bash
g++ server.cpp -o server
g++ client.cpp -o client
```

### 2\. Create the Directories

You must create the folders that the server and client will use:

```bash
mkdir server_files
mkdir client_downloads
```

### 3\. Start the Server

Run the compiled server executable in a terminal:

```bash
./server
```

The server will start and listen on **port 65432**.

### 4\. Run the Client

Open another terminal and run the compiled client executable:

```bash
./client
```

The client will connect to the server.

  * **Password:** When prompted, enter the password (the hardcoded one is `mehraj123`).
  * **Commands:** You will then see the command interface.

-----

## 💻 Client Commands

| **Command** | **Description** |
| :--- | :--- |
| `LIST` | Displays all available files on the server. |
| `GET <filename>` | Downloads the specified file from the server. |
| `PUT <filename>` | Uploads the specified file to the server. |
| `QUIT` | Ends the client session. |

-----

## 🧭 Future Scope

  * Add **multi-client handling** using threading or `select()`.
  * Implement **advanced encryption (SSL/TLS)** using a library like OpenSSL.
  * Include **GUI** for better usability (e.g., with Qt or wxWidgets).
  * Add **integrity verification** for transferred files (e.g., using an MD5 or SHA-256 hash).

-----

⭐ *A simple yet powerful C++ networking project demonstrating file transfer over sockets.*
