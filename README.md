# ZenRace - TCP Server
## Project
ZenRace is a project that was conducted in the context of a mentored project during our final year of the Bachelor in Computer Science at the IUT Nord Franche-Comté. The main objective of this project is to developp a complete IOT system that allows to manage a running race. This system is composed of several parts:
- A REST API that allows to manage the data of the project.
- A web application that allows to manage
- A mobile application that allows spectators to follow the race and share photos of the event.
- A set of IOT devices that allow to get the data of the race.

## Description
**This repository contains the TCP server of the ZenRace project.** This server is responsible for managing the communication between the IOT devices and the API. It allows to receive the data.

## Installation
### Prerequisites
To run the API, you need to have the following tools installed on your machine:
- Maven
- Java (We recommend using the latest LTS version)
- MongoDB

## Configuration
The configuration of the API is done in environment variables. You can create a `.env` file at the root of the project and define the following variables:
- `TCP_SERVER_PORT`: The port on which the server will listen for incoming connections. Default value: `3000`.
- `MONGODB_URI`: The URI of the MongoDB database. Default value: `mongodb://localhost:27017/zenrace`.

## Usage
Maven is configured to execute the server using the 'exec-maven-plugin' plugin. You can run the server using the following command:
```bash
mvn exec:java
```

## Documentation
