# 🌐 Client Gateway

> [!NOTE]
> The Client Gateway is the communication point between our clients and services. It is responsible for receiving requests, forwarding them to the appropriate services, and returning the response to the client.

## 📦 Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/Nest-Microservices-Application/client-gateway
    cd client-gateway
    ```

2. **Install dependencies:**

    ```sh
    npm install
    ```

3. **Configure environment variables:**

    Copy the `.env.template` to `.env` and update the environment variables as needed.

4. **Start the NATS server:**

    If you are not using `products-launcher` to run the Docker images and are starting each project individually, ensure that the NATS server is running:

    ```sh
    docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
    ```

5. **Start the project:**

    ```sh
    npm run start:dev
    ```

> [!IMPORTANT]
> The NATS server is only required if you are not using `products-launcher` with Docker images and are running each project individually.
