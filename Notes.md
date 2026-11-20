
# Networking Notes

## 1. OSI Model

The OSI model consists of seven layers that explain how data is transmitted between devices across a network.

- **Layer 1 – Physical:** Transmits bits through cables, fibre or wireless signals.
- **Layer 2 – Data Link:** Uses frames and MAC addresses to deliver data to devices within the same local network.
- **Layer 3 – Network:** Introduces IP addresses and routing, allowing devices to communicate across different networks.
- **Layer 4 – Transport:** Uses TCP for reliable, ordered delivery and UDP for low-overhead communication, often used in real-time applications.
- **Layer 5 – Session:** Establishes and manages communication sessions.
- **Layer 6 – Presentation:** Handles data formatting, encoding and encryption.
- **Layer 7 – Application:** Provides networking services through protocols such as HTTP, HTTPS, SSH and FTP.

## 2. Ports and Protocols

Ports help direct network traffic to the correct application or service.

- **HTTP – Port 80:** Web communication.
- **HTTPS – Port 443:** Secure, encrypted web communication.
- **SSH – Port 22:** Secure remote access.
- **FTP – Port 21:** File transfer control.

## 3. Firewalls

Firewalls protect devices and networks by controlling inbound and outbound traffic through security rules.

- **Inbound rules:** Control incoming traffic.
- **Outbound rules:** Control outgoing traffic.
- **Stateful firewall:** Tracks active connections and automatically recognises related return traffic.
- **Stateless firewall:** Checks packets individually without remembering previous connections. Return traffic must be allowed by the relevant rules.

Firewall rules can be configured using IP addresses, ports and protocols.

## 4. DNS (Domain Name System)

DNS translates domain names into IP addresses, allowing devices to locate servers.

### DNS Lookup Process

1. **Local device:** Checks its DNS cache and local hosts file for the requested address.
2. **Recursive resolver:** Receives the DNS query and checks whether the answer is already cached.
3. **Root DNS server:** If the answer isn't cached, the resolver contacts a root server, which directs it to the appropriate TLD server.
4. **TLD server:** Directs the resolver to the authoritative name server responsible for the domain, such as one ending in `.com` or `.co.uk`.
5. **Authoritative DNS server:** Provides the requested DNS record, such as an A record containing an IPv4 address.
6. **Caching:** The recursive resolver returns the answer to the device and caches it for future requests until the TTL expires.

## 5. What I Learnt

Through this module, I developed a better understanding of how devices communicate across networks, from transmitting data through the OSI layers to using IP addresses, ports and protocols.

I also learnt how DNS resolves domain names into IP addresses and how stateful and stateless firewalls help control network traffic.
