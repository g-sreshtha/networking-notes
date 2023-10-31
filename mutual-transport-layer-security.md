# Mutual Transport Layer Security (mTLS) - What is it?

Before understanding what mTLS is, we must define Transport Layer Security (TLS). TLS is a cryptographic protocol that provides security through end to end encryption for communications over computer networks and the Internet. The primary use for TLS is encrypting communications over web servers and applications as well as being widely used in applications such as email and instant messaging. In a nutshell, it authenticates the server in a client server connection and encrypts communications between client and server so that external parties cannot spy on the communications. 

There are **three** main components to the TLS protocol:
- **Encryption**: which hides important data to public users and third parties. TLS handshakes, which is a process that kicks off a communication session that uses TLS, use public key cryptography like RSA or Diffie-Hellman to authenticate the identitiy of the origin server. 
- **Authentication**: which ensures that the parties exchanging information are the correct recipients and senders. In this process, a TLS certificate is used to authenticate the server's or the device's identity. This is a data file that contains important information that helps verify those identities as well as a statement of who issued the certificate and the certificate's expiry date.
- **Integrity**: verifies whether the data has not been forged or tampered with. This is where the TLS handshake process verifies the TLS certificate and the possession of the private key from the server.

**Mutual TLS**, also known as two-way TLS, is a security protocol where server and client authenticate eachother before establishing a secure connection. This is different from TLS where the client authenticates the server only. In this protocol both client and server presents a TLS certificate and they both verifies eachother's certificates and the server grants access to the client. In the end, like the TLS protocol, they exchange information over encrypted TLS connection. 

***To implement mTLS, both the client and server must have a TLS certificate. The certificate contains the public key of the owner and is signed by a trusted certificate authority (CA), for example BastionXP CA.***
Solarized dark             |  Solarized Ocean
:-------------------------:|:-------------------------:
hi  |  hello



## Example application which uses mTLS
- Amazon Web Servers (AWS) uses it to secure communation between their services and clients.
- Netflix uses it to secure communication between their microservices in its IT datacenters.
- Tesla uses mTLS to secure communication between its cars and its servers.
- The US Department of Defense is using mTLS to secure communication between its systems and its contractors' systems.

