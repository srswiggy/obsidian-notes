> Request is taking a while, I'll check with you later

## Request/Response isn't ideal for - 
- Used when Request is taking a long time to process
	- Ex - Upload a youtube video
- The backend want to send notifications
	- A user just logged in

## Short Polling
- Client sends a request
- Server responds immediately with a handle (job ID)
- Server continues to process the request
- Client uses that handle to check for status of the processing
- Multiple "short" request response as polls

### Pros
- Simple to Implement
- Good for long running requests
- Client can disconnect

#### Cons
- To "chatty" i.e. too much communication between client-server
- Takes network bandwidth
- wasted backend resources
- can't use caching