# tinyRedis
![tinyRedis Logo](logo.png)


Welcome to tinyRedis, a minimalistic Redis-compatible server implementation written in Go. This project is designed to be lightweight, efficient, and fully compatible with the Redis protocol, making it suitable for educational purposes, testing, and small-scale deployments.
## Features

- **Redis Protocol Compatibility:** Implements key features of the Redis protocol to ensure compatibility with existing Redis clients.
- **Lightweight Design:** Focused on core functionality with minimal overhead, making it fast and easy to deploy.
- **Written in Go:** Leverages Go's concurrency model for efficient handling of multiple connections and data safety.

## Getting Started
### Prerequisites
Before you begin, ensure you have Go installed on your machine. You can download and install Go from [https://golang.org/dl/](https://golang.org/dl/).
### Installing
To install tinyRedis, clone the repository and build the project:
```bash
git clone https://github.com/yourusername/tinyRedis.git
cd tinyRedis
go build .
```
## Running tinyRedis
To start the server, simply run:
```bash
./tinyRedis
```
tinyRedis will listen on port 6379, you can connect to it using any standard Redis client.
### Example usage
Here is a simple example of setting a key and retrieving it using a Redis client in Python:
```python
import redis

# Connect to the server
client = redis.Redis(host='localhost', port=6379, decode_responses=True)

# Set a key
client.set('admin', 'robitec')

# Get the key
print(client.get('admin'))  # Output: robitec
```
## Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.



