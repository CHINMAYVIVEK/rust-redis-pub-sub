# rust-redis-pub-sub

This project demonstrates a simple Pub/Sub (Publish/Subscribe) integration with Redis using Rust. It includes examples of a Redis publisher and subscriber, showcasing how to send and receive messages. Redis is run using Docker for ease of setup and management.

## Features

- **Redis Publisher**: Sends messages to a Redis channel.
- **Redis Subscriber**: Listens for messages from a Redis channel and processes them.
- **Dockerized Redis**: Uses Docker to simplify the setup and management of Redis.

## Prerequisites

- Rust (latest stable version recommended)
- Docker and Docker Compose
- Cargo (Rust's package manager)

## Getting Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/chinmayvivek/rust-redis-pub-sub.git
cd rust-redis-pub-sub
```

### Step 2: Build the Rust Project

```bash
cargo build
```

### Step 3: Setup Redis using Docker

1. **Ensure Docker is installed and running on your system**.
2. **Start Redis**:

   ```bash
   docker run -d  -p 6379:6379 redis
   ```


### Step 4: Run the Subscriber

Open a terminal and run:

```bash
cargo run --quiet
```

## Usage

1. **Publish messages**: The publisher sends messages to a Redis channel.
2. **Subscribe to messages**: The subscriber listens for messages on the same Redis channel and processes them as they arrive.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Redis](https://redis.io/)
- [redis-rs crate](https://docs.rs/redis/)
- [Docker](https://www.docker.com/)
