# TCP/IP Fundamentals

## Introduction

TCP/IP is the family of protocols used for communication across the internet and many private networks. It is commonly described using four layers: Application, Transport, Internet, and Network Access.

## IP

Internet Protocol (IP) provides addressing and routing so packets can travel between networks. IP itself does not guarantee that packets arrive or arrive in order.

## TCP

Transmission Control Protocol (TCP) is connection-oriented. It uses mechanisms such as sequence numbers, acknowledgements, and retransmission to provide reliable, ordered delivery of a byte stream.

## UDP

User Datagram Protocol (UDP) is connectionless and has less transport-level overhead. It does not itself guarantee delivery, ordering, or retransmission.

## TCP and UDP comparison

| TCP | UDP |
|---|---|
| Connection-oriented | Connectionless |
| Reliable, ordered byte stream | No built-in delivery or ordering guarantee |
| Uses acknowledgements and retransmission | Lower protocol overhead |
| Commonly used by web and file-transfer applications | Commonly used by DNS queries, voice, and streaming applications |

The actual protocol used depends on the application and configuration.

## Security connection

Knowing whether traffic uses TCP or UDP is useful when reading network information and interpreting firewall rules or packet captures. The protocol alone does not prove that traffic is safe or malicious; context is needed.

## What I am learning

I am learning how IP addressing and routing differ from transport-layer communication, and how TCP and UDP provide different transport behaviours.
