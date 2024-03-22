### Steps
- Client sends a Request
- Server parses the Request
- Server processes the Request
- Server sends a Response

### Where it is used?
- Web, HTTP, DNS, SSH
- RPC
- SQL and Database Protocols
- REST/GraphQL/SOAP

## Anatomy of a Request / Response
- A request structure is defined by both client and server
- Request has a boundary
- Defined by a protocol and a message format
- Same for response

![Impact of Three-way Handshake and Slow Start Algorithm - GeeksforGeeks](https://media.geeksforgeeks.org/wp-content/uploads/20220303134334/impactofssrand3whssecond-660x626.jpg)

### Doesn't work everywhere
- Notification Service
- Chatting Application
- Very Long processing request
# Demo 
```zsh
curl -v --trace out.txt http://google.com
```
