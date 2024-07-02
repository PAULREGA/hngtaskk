# Weather Server API

This is a simple Express.js application that provides a weather greeting based on the user's IP address.

## Features

- Greets users by name (if provided) or as "Guest"
- Retrieves the user's location and current temperature based on their IP address
- Uses the WeatherAPI to fetch weather data

## Prerequisites

- Node.js
- npm (Node Package Manager)

## Installation

1. Clone this repository
2. Run `npm install` to install dependencies

## Configuration

1. Create a `.env` file in the root directory
2. Add your WeatherAPI key to the `.env` file:

## Usage

1. Start the server:

2. The server will run on `http://localhost:3000` (or the port specified in your environment)

## API Endpoint

### GET /api/hello

Returns a greeting with the current weather for the user's location.

Query Parameters:
- `visitor_name` (optional): The name of the visitor

Response:
```json
{
"client_ip": "user's IP address",
"location": "user's location",
"greeting": "Hello, [name]! The temperature is [temp] degrees Celsius in [location]"
}