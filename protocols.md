# Networking Protocols


### TCP
The **Transmission Control Protocol (TCP)** is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it **complemented the Internet Protocol (IP)**. Therefore, the entire suite is commonly referred to as **TCP/IP**. TCP **provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network**. Major internet applications such as the `World Wide Web`, `email`, remote administration, and file transfer rely on `TCP`, which is part of the Transport Layer of the `TCP/IP` suite. `SSL/TLS` often runs on top of TCP.

### Internet Control Message Protocol

The **Internet Control Message Protocol (ICMP)** is a supporting protocol in the Internet protocol suite. It is used by network devices, including routers, to send error messages and operational information indicating success or failure when communicating with another IP address, for example, an error is indicated when a requested service is not available or that a host or router could not be reached.

* [Wikipedia](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol)

### SMTP
The **Simple Mail Transfer Protocol (SMTP)** is a communication protocol for electronic mail transmission. As an Internet standard, SMTP was first defined in 1982 by RFC 821, and updated in 2008 by RFC 5321 to Extended SMTP additions, which is the protocol variety in widespread use today. Mail servers and other message transfer agents use SMTP to send and receive mail messages. SMTP servers commonly use the **Transmission Control Protocol on port number 25**.