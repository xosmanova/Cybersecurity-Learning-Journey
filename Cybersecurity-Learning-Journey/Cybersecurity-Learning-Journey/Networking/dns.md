# DNS Fundamentals

## What is DNS?

The Domain Name System (DNS) translates domain names, such as `example.com`, into information used by computers to reach services. A common DNS task is finding the IP address associated with a domain name.

## Basic resolution process

At a high level:

1. An application needs to look up a domain name.
2. The device checks available local or cached information.
3. If needed, it asks a configured DNS resolver.
4. The resolver obtains the required answer through the DNS system.
5. The answer is returned and may be cached for a period of time.

The exact process depends on caching, resolver configuration, and the type of DNS query.

## Common DNS record types

| Record | Purpose |
|---|---|
| A | Maps a name to an IPv4 address |
| AAAA | Maps a name to an IPv6 address |
| CNAME | Makes one name an alias of another name |
| MX | Identifies mail servers for a domain |
| NS | Identifies authoritative name servers |
| TXT | Stores text data, often used for domain verification and email security policies |

## Security connection

DNS information can be useful during defensive investigations. For example, analysts may review domain lookups associated with a device and compare them with other available evidence. An unfamiliar domain is not automatically malicious; it needs context and verification.

## What I am learning

I am learning how domain names are resolved, what common DNS records mean, and why DNS activity can be useful during network investigations.
