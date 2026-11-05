# The OSI Model

## Introduction

The Open Systems Interconnection (OSI) model is a reference model that describes network communication in seven layers. It helps people discuss where a networking function takes place and troubleshoot communication problems.

## The seven layers

| Layer | Name | Main idea | Examples |
|---|---|---|---|
| 7 | Application | Network services used by applications | HTTP, DNS |
| 6 | Presentation | Data representation, encoding, and encryption concepts | Data formats, TLS-related presentation concepts |
| 5 | Session | Establishing and managing communication sessions | Session management |
| 4 | Transport | End-to-end transport between hosts | TCP, UDP |
| 3 | Network | Logical addressing and routing | IP, routers |
| 2 | Data Link | Communication on a local link | Ethernet, MAC addresses |
| 1 | Physical | Signals and physical media | Cables, radio signals |

The OSI model is a teaching and troubleshooting model. Real-world network protocols do not always fit neatly into only one layer.

## Why it is useful

When investigating a connection problem, the model provides a way to organise questions. For example:

- Is the physical connection available?
- Can the device communicate on the local network?
- Is IP routing working?
- Is the transport connection established?
- Is the application responding?

## Security connection

Understanding the layers helps when describing where a security control or network event occurs. For example, IP addresses are associated with the network layer, while TCP and UDP operate at the transport layer.

## What I am learning

I am learning the purpose of each OSI layer and using the model as a framework for understanding network communication.
