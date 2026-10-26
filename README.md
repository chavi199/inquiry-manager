# Inquiry manager

A Java client-server system for customer inquiries. The server accepts several clients at once. Each connection is handled on its own thread. An inquiry can be a question, a request, or a complaint, and it is assigned to a representative.

The server listens on port `8888`. The client opens a socket to that port, sends a request object, and reads the response.

Records are written to files through a small persistence layer (`HandleFiles`), including representative data in CSV.

## Stack

- Java
- Sockets and threads
- IntelliJ IDEA

## Layout

```text
ClientSide1/                                      client
IntelliJTraining_inquirymanager_chanadavidov1/    server, business logic, and file storage
```

Open the two modules in IntelliJ. Start the server, then start the client.

## Branches

`main` contains the merged client and server work. `feature/get-agents-count` adds a count of representatives and is one commit ahead of `main`.
