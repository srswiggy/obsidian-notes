> Request is taking long, I'll check with you later but talk to me only when it's ready

#### Kafka uses Long Polling

## What is long Polling
- Client sends a request
- Server responds immediately with a handle (Job ID)
- Server continues to process the request
- Client uses that handle to check status
- Server DOES NOT reply until it has the response
- So we got a handle, we can disconnect a client

### Pros
- Less chatty and backend friendly
- Client can still disconnect

### Cons
- Not real time