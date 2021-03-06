# Computer Systems: A Programmer's Perspective
## Chapter 7 Linking 
### 7.1 Compiler Drivers 
### 7.2 Static Linking 
### 7.3 Object Files 
### 7.4 Relocatable Object Files 
### 7.5 Symbols and Symbol Tables 
### 7.6 Symbol Resolution 
### 7.7 Relocation 
### 7.8 Executable Object Files 
### 7.9 Loading Executable Object Files 
### 7.10 Dynamic Linking with Shared Libraries 
### 7.11 Loading and Linking Shared Libraries from Applications 
### 7.12 Position-Independent Code (PIC)
### 7.13 Library Interpositioning 
### 7.14 Tools for Manipulationg Object Files 
### 7.15 Summary 

## Chapter 10 System-Level I/O
### 10.1 Unix I/O
Operating files. All application announces its intention to access an I/O device by asking the kernel to open the corresponding file. The kernel returns a small nonnegative integer, called a descriptor, that identifies the file in all subsequent operation on the file. The kernel keeps track of all information about the open file. The application only keeps track of the descriptor. 

### 10.2 Files 
### 10.3 Opening and Closing Files 
### 10.4 Reading and Writing Files 
### 10.5 Robust Reading and Writing with the RIO Package 
### 10.6 Reading File Metadata 
### 10.7 Reading Directory Contents 
### 10.8 Sharing Files 
### 10.9 I/O Redirection 
### 10.10 Standard I/O
### 10.11 Putting It Together: Which I/O Functions Should I Use? 
### 10.12 Summary 
## Chapter 11 Network Programming 
### 11.1 The Client-Server Programming Model 
### 11.2 Networks 
### 11.3 The Global IP Internet 
#### 11.3.1 IP Addresses 
#### 11.3.2 Internet Domain Names 
#### 11.3.3 Internet Connections 
A connection is point-to-point in the sense that it connects a pair of processes. 

A socket is an end point of a connection. Each socket has a corresponding socket addres that consists of an Internet addres and a 16-bit integer port and is denoted by the notation address:port. 

### 11.4 The Sockets Interface 
The socket interface is a set of functions that are used in conjunction with the Unix I/O functions to build network applications. 

#### 11.4.1 Socket Address Structures 
From the perspective of the Linux kernel, a socket is an end point for communication. From the perspective of a Linux program, a socket is an open file with a corresponding descriptor. 

Internet socket addresses are stored in 16-byte structure having the type sockaddr_in, shown in Figure 11.13. 
#### 11.4.2 The socket Function 
#### 11.4.3 The connect Function 
#### 11.4.4 The bind Function 
#### 11.4.5 The listen Function 

#### 11.4.6 The accept Function 
#### 11.4.7 Host and Service Conversion 
#### 11.4.8 Helper Functions for the Socket Interface 

## Chapter 12 Concurrent Programming 
### 12.1 Concurrent Programming with Processes 
### 12.2 Concurrent Programming with I/O Multiplexing 
### 12.3 Concurrent Programming with Threads 
### 12.4 Shared Variables in Threaded Programs 
### 12.5 Synchronizing Threads with Semaphores 
### 12.6 Using Threads with Semaphores 
### 12.7 Other Concurrency Issues
### 12.8 Summary 
