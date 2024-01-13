# Hyper Status

A tiny package for http status code.

## Getting Started

To tnstall `Hyper Status` in your project.

```bash
pnpm install hyper-status
```

<br />

## Examples

```ts
import fastify from "fastify";
import hyperstatus from "hyper-status";

const server = await fastify();

server.get("/", (request, reply) => {
  reply
    .code(hyperstatus.HTTP_202_ACCEPTED)
    .send({ message: "Server is Okey" })
})

server.listen();
```