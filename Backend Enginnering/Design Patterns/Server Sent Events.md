> One Request, a very very long response
> You send one request, and the server keeps sending you a response and does not stop effectively making it a stream

## Limitations of Request/Response
- Vanilla Req/Res isn't ideal for notification backend
- Client wants real time notification from backend
	- A user just logged in
	- A message is just received
- Push works but restrictive
- Server Sent Events work with Req/Res

## What is Server Sent Events
- A response has start and end
- Client sends a request
- Server sends logical events as part of response
- Server never write the end of the response
- It is still a request but an unending response
- Client parses the streams data looking for data
- Works with req/res (HTTP)

### Pros
- Real time
- Compatible with Request/Response

### Cons
- Clients must be online
- Clients might not be able to handle
- Polling is preferred for light client
- HTTP/1.1 problem (6 connections limit to a domain by Chrome and rest browsers follows that)