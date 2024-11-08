# WebSocket Client Application in C++

This project is a WebSocket client application developed in C++ to handle secure WebSocket (WSS) connections. The client is built using the Boost.Beast library for WebSocket communication, and it is configured with the GN build system. The application supports CLI-based interactions and can be easily integrated into larger systems or used for standalone communication over WebSockets.

## Features

- **WebSocket Communication**: Supports both WebSocket (WS) and secure WebSocket (WSS) connections.
- **Boost.Beast**: Uses the Boost.Beast library for efficient WebSocket client functionality.
- **CLI Interface**: The client is operated through a command-line interface (CLI) with options for connection, message sending, and other WebSocket actions.
- **GN Build System**: The project is built using the GN build system for seamless compilation and integration.

## Requirements

- C++17 or later
- Boost 1.70 or later (with Beast library)

### Optional

- OpenSSL (for WSS support)

### Setup

## Clone the repository

```bash
git clone https://github.com/0xakhii/WebSocketClient
cd WebSocketClient
```
### Build the application
  *1-Install dependencies: Ensure that you have Boost, g++, and OpenSSL installed (if using WSS).*
```bash
sudo apt update -y && sudo apt install libboost-all-dev \
 && sudo apt install build-essential && sudo apt install openssl
```
### 2-Generate excutable file:
 *By running the follwing command in your Terminal*
``` bash
g++ -std=c++17 -o WebSocketClient main.cpp WebSocketClient.cpp -lboost_system -lboost_thread -lssl -lcrypto -pthread
```
### 3-Run the application
 *To run the WebSocket client application, use the following command in your terminal:*
```bash
./WebSocketClient -u wss://echo.websocket.org
```
## Contribution

1. Fork this repository.
2. Create a feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
