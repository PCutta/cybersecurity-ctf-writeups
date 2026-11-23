# what's a net cat? — Introduction to Netcat

**Platform:** CyLab Security Academy
**Category:** General Skills
**Difficulty:** Easy
**Status:** Solved

## Challenge Objective

Use Netcat (`nc`) to establish a connection to a remote server and retrieve the challenge flag.

## Environment

- CyLab Security Academy browser-based Linux workspace
- Linux terminal
- Netcat (`nc`)
- Remote TCP service

## Approach

### 1. Identify the Connection Information

The challenge provided a hostname and port number for a remote service.

The command structure was:

```bash
nc <hostname> <port>
```

The hostname identifies the destination server, while the port identifies the service to connect to.

### 2. Explore the Netcat Command

I initially entered:

```bash
nc
```

Because I did not specify a destination, Netcat displayed its usage information.

This helped me understand that additional arguments were required.

### 3. Connect to the Remote Server

I then entered the complete command using the challenge's hostname and port:

```bash
nc xebec.cylabacademy.net 33293
```

The command established a connection to the remote challenge service.

### 4. Retrieve the Flag

After connecting, the server displayed a message containing the challenge flag.

I copied the flag and submitted it through CyLab Security Academy.

The platform confirmed that the challenge was solved.

## Result

Successfully connected to a remote TCP service using Netcat and retrieved the challenge flag.

## Skills Practiced

- Using Netcat (`nc`)
- Working with Linux terminal commands
- Understanding hostnames and ports
- Establishing TCP connections
- Reading command-line usage information
- Troubleshooting incomplete commands
- Interacting with remote network services

## What I Learned

This challenge introduced me to Netcat, a command-line networking utility.

I learned that network connections require a destination hostname or IP address and a port number.

I also learned how command-line tools display usage information when required arguments are missing.

Netcat is useful for network troubleshooting, connectivity testing, and cybersecurity exercises.

This challenge helped strengthen my understanding of basic networking concepts and Linux command-line tools.
