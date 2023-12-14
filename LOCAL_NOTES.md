# Working with Microservices in Go (Golang)

Build highly available, scalable, resilient distributed applications using Go

## Section: Introduction
### Introduction
#### Working with microservices in Go
  > Building scalable, resilient, distributed applications
#### Microservices
- Monolithic applications
  - All logic exists in one application
  - Everything is handled by one application
    - User authentication
    - Sending email
    - Logging
    - All business logic
- Distributed applications
- Microservices
  - Loosely coupled services
  - Breaking monolithic up applications from functions/packages to completely separate programs
  - Communicate via JSON/REST, RPC, gRPC, messaging queue, etc.
  - Easier to scale
  - Easier to maintain
  - Harder to write
> Do one thing, and do it well (The Unix philosophy)

#### What we'll build

- A front end web application that connects to five Microservices
  - **Broker** - optional single point of entry microservices
  - **Authentication** - Postgres
  - **Logger** - MongoDB
  - **Mail** - sends email with a specific template
  - **Listener** - consumes messages in RabbitMQ and initiates a process 

- We'll communicate between Microservices using
  - REST API with JSON as transport
  - Sending and Receiving using RPC
  - Sending and Receiving using gRPC
  - Initiating and responding to events using Advanced Message Queueing Protocol (AMQP)

### About me

### Installing Go

- Setup for windows:
  ```powershell
  winget install -e --id GoLang.Go
  ```

### Installing Visual Studio Code

- Setup for windows:
  ```powershell
  winget install -e --id Microsoft.VisualStudioCode
  ```
- You want to make sure all the `Go: Install/Update Tools` are enabled
- Suggestion: Also install extension: `gotemplate-syntax`

### Installing JetBrains Toolbox (GoLand)
- Setup for windows:
  ```powershell
  winget install -e --id JetBrains.Toolbox
  ```

### Installing Make

- Setup for windows:
  ```powershell
  winget install -e --id GnuWin32.Make
  ```

### Installing Docker

- Setup for windows:
  ```powershell
  winget install -e --id Docker.DockerDesktop
  ```

### Asking for help

### Mistakes. We all make them

## Section: Building a simple front end and one Microservice

### What we'll cover in this section
> Setup of a very simple Microservice; the broker service in Docker



















## Section: Building an Authentication Service
## Section: Building a Logger Service
## Section: Building a Mail Service
## Section: Building a Listener service: AMQP with RabbitMQ
## Section: Communicating between services using Remote Procedure Calls (RPC)
## Section: Speeding things up (potentially) with gRPC
## Section: Deploying our Distributed app using Docker Swarm
## Section: Deploying our Distributed app to Kubernetes
## Section: Testing Microservices
## Section: Final thoughts
