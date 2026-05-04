# learn-pub-sub-typescript-starter (Peril)

This repo contains the TypeScript starter code for the "Peril" application for the [Learn Pub/Sub](https://www.boot.dev/courses/learn-pub-sub-rabbitmq-typescript) course on Boot.dev.

## Local Development

Make sure you're on Node version 22+.

### Prerequisites

- [Docker](https://www.docker.com/) is required to run the RabbitMQ message broker.

### Start RabbitMQ

```bash
npm run rabbit:start
```

This starts a RabbitMQ container (`peril_rabbitmq`) exposed on ports `5672` (AMQP) and `15672` (management UI).

You can view the RabbitMQ management dashboard at http://localhost:15672 (default credentials: `guest` / `guest`).

### Run the server and client

In one terminal, start the game server:

```bash
npm install
npm run server
```

In another terminal, start a game client:

```bash
npm run client
```

You can run multiple clients simultaneously to simulate multiple players.

### Other commands

| Command               | Description                  |
| --------------------- | ---------------------------- |
| `npm run rabbit:stop` | Stop the RabbitMQ container  |
| `npm run rabbit:logs` | Tail RabbitMQ container logs |
| `npm run build`       | Compile TypeScript           |
| `npm run format`      | Format code with Prettier    |

Michiel's version of Boot.dev's Peril app. Created for learning and demonstration purposes.

## License

MIT License.

---

_Created for learning and demonstration purposes._
