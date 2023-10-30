# Mutual Transport Layer Security (mTLS) - What is it?

Before understanding what mTLS is, we must define Transport Layer Security (TLS). TLS is a cryptographic protocol that provides security through end to end encryption for communications over computer networks and the Internet. The primary use for TLS is encrypting communications over web servers and applications as well as being widely used in applications such as email and instant messaging. 

There are **three** main components to the TLS protocol:
- **Encryption**
- **Authentication**
- **Integrity**


***To implement mTLS, both the client and server must have a TLS certificate. The certificate contains the public key of the owner and is signed by a trusted certificate authority (CA), for example BastionXP CA.***



## Example application which uses mTLS
- Amazon Web Servers (AWS) uses it to secure communation between their services and clients.
- Netflix uses it to secure communication between their microservices in its IT datacenters.
- Tesla uses mTLS to secure communication between its cars and its servers.
- The US Department of Defense is using mTLS to secure communication between its systems and its contractors' systems.

