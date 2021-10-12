### TLS handshake
 - client -> server: Hello + supported encryption method?
 - server -> client: choose cypher based client msg, send Hello
 - server -> client: certificate include **public key**
 - server -> client: send hello done
 - client -> server: key exchange by send pre-master secret encrypted with server public key, start generating **symmatric key** for further communicate, notify server
 - server -> client: server decrypt cypher to get the same **symmatric key**, and notify the client
 - from now on, two side have the same **symmatric key** to communicate encrypted data
---
TLS requires a reliable transport. On the internet, this leaves only TCP, as UDP does not offer reliability.
TLS does require a reliable transport because (in compliance with the layered architecture of the ISO/OSI reference model) it does not handle transport errors, lost packets or other disturbances that may occur with IP.
TLS is designed to offer a secure channel on top of a reliable transport and it does this quite well. DTLS does (I assume) the necessary error handling within the protocol.