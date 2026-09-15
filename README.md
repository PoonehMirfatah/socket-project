# Java Socket Chatroom

A multi-client chatroom implemented with Java sockets and MySQL persistence. The project contains a server and two sample clients, with serializable models for users, public messages, and private messages.

## Features

- TCP server listening on port `8080`
- A dedicated thread for each connected client
- User sign-up and login models
- Public and private messages
- Online-user session tracking
- MySQL-backed user and message operations

## Structure

```text
ConsuleProject/
|-- Server/   # Socket server, sessions, and server-side models
|-- Client1/  # First example client
`-- Client2/  # Second example client
```

## Running the project

1. Install a Java Development Kit and MySQL.
2. Create the database expected by the application and add MySQL Connector/J to the classpath.
3. Replace the local database settings in each `MySQLConnection.java` with environment-specific values.
4. Start `View.Server`.
5. Start one or both `View.Client` applications in separate terminals or IDE run configurations.

## Security note

The current code is a course prototype. Database configuration is embedded in source files and SQL statements are constructed directly; use environment variables and parameterized queries before adapting it for production.

## Academic context

This project demonstrates client-server networking, concurrency, object serialization, session tracking, and relational data access in Java.
