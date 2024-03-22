## Request/Response isn't always ideal

- Client wants real time notification from backend
	- A user just logged in
	- A message is just received

## What is Push?
- Client connects to a server
- Server sends data to the client
- Client doesn't have to request anything
- Protocol must be bi-directional
- Used by **RabbitMQ**

## Pros & Cons
### Pros
- Real-time
### Cons
- Clients must be online and connected to the server
- Clients might not be able to handle
- Requires a bi-directional protocol
- Polling is preferred for light clients