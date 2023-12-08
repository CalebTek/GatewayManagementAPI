# Gateway Management REST API

This project provides a RESTful API for managing gateways and their associated devices. It allows users to store information about gateways, validate their attributes, and perform operations on peripheral devices.

For the frontend counterpart, please refer to the [GatewayManagementUI](https://github.com/CalebTek/GatewayManagementUI.git) repository.

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
```

## API Endpoints

### Create Gateway

```http
POST /api/gateway/gateways
```

Create a new gateway by providing JSON data in the request body.

Example:

```json
{
  "serialNumber": "GW123",
  "name": "Main Gateway",
  "ipv4Address": "192.168.1.1"
}
```

### Get All Gateways

```http
GET /api/gateway/gateways
```

Retrieve information about all stored gateways.

### Get Gateway by ID

```http
GET /api/gateway/gateways/{id}
```

Retrieve details about a single gateway by providing its ID.

## Contributions

Contributions are welcome. Please fork the repository, make your changes, and submit a pull request.

