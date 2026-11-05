# Common Network Protocols and Ports

A protocol defines rules for communication. Some commonly encountered protocols use well-known default port numbers.

| Protocol | Common port | Purpose |
|---|---:|---|
| HTTP | TCP 80 | Web traffic |
| HTTPS | TCP 443 | Encrypted web traffic |
| DNS | 53 | Domain name queries; commonly UDP and also TCP |
| SSH | TCP 22 | Secure remote command-line access |
| FTP | TCP 21 | File transfer control connection |
| SMTP | TCP 25 | Mail transfer between servers |
| RDP | TCP/UDP 3389 | Remote Desktop access |

These are common defaults, not guarantees. Services can be configured to use other ports, and a port number alone does not identify exactly what an application is doing.

## Why ports matter

Ports help a device distinguish between different network services. When reviewing firewall rules or network connection information, it is useful to know which services commonly use particular ports.

## Security connection

Exposed services should be understood and managed. Organisations generally limit network access to the services that are required and monitor unexpected activity. Any review should be performed only on systems and networks where permission has been granted.

## What I am learning

I am learning to recognise common protocols and their default ports, while remembering that port numbers need to be interpreted alongside other evidence.
