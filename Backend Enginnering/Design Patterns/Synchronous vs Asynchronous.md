# Synchronous I/O
- Caller sends a request and blocks
- Caller cannot execute any code meanwhile
- Receiver responds, Caller unblocks
- Caller and Receiver are in "sync"

# Asynchronous I/O
- Caller sends a request
- Caller can work until it gets a response
- Caller either:
	- Checks if the response is ready (**epoll in linux**, node js also use epoll in linux)
	- Receiver calls back when it's done (**io_uring** in linux)
	- Spins up a new thread that blocks
- Caller and receiver are not in sync

# Sync vs Async in real life
- Sync - Asking someone a question in a meeting and not able to move foreword without the answer.
- Async - Asking someone a question in an email and after sending email, you continue working and when they revert back, you use that information.