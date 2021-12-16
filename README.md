# JChat

Lightweight team chat written in C++.  Based heavily on "messenger" by AraKhachatryan, JChat is a command line chat program for Linux/Unix that allows for quick communcation between users on the same LAN.   JChat is meant to be extremely portable, and has no encryption and makes no attempt to obfuscate messages.  It is meant to be used on a secure network where privacy/encryption is handled by the netowrk (aka Wireguard or OpenVPN).  It is particuleraly useful as lightweight communcations in Red Team engagements. 


## Files
- README.md - the current readme file
- client.cpp - multithreaded client with POSIX sockets for Linux/Unix terminal command line messenger
- encode_decode.cpp	- functions definations for encodeing and decoding messages for sending over TCP socket
- encode_decode.hpp	- functions declarations for encodeing and decoding messages for sending over TCP socket
- makefile - compiling and bild automation with GNU make
- namespace_terminal.hpp - designed for manipulating with linux terminal
- server.cpp - Multi client and multithreaded server with POSIX sockets for Linux/Unix terminal command line messenger

## Requirements
- g++ compiler with C++11 standart
- Supporting POSIX standarts
- GNU make

## Compilation:

Compilation is done with GNU make, just type on terminal "make"

## Usage:

- on server side: ./server

- on client side: ./client  server_IPv4_address
