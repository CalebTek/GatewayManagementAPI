# Gateway Management REST API

This project provides a RESTful API for managing gateways and their associated devices. It allows users to store information about gateways, validate their attributes, and perform operations on peripheral devices.

## Features

- Create a new gateway
- Display information about all stored gateways (and their devices)
- Display details about a single gateway
- Add and remove a peripheral device from a gateway

## Technologies Used

- C# with ASP.NET Core
- In-memory storage (for simplicity, replace with a database in production)
- JSON format for input/output data
- Unit tests for validation

## How to Run

1. Clone this repository.
2. Open the project in your preferred C# IDE.
3. Build the solution.
4. Run the application.

Ensure you have the necessary .NET SDK installed.

```bash
$ dotnet build
$ dotnet run
