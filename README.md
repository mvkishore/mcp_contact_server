# MCP Contact Server and Chat Bot Integration

This project implements a Message Control Protocol (MCP) server that serves contact information for requested phone numbers, along with a web-based chat bot application that integrates with the MCP server.

## Project Structure

- `/mcp_server/` - The MCP server implementation
- `/web_app/` - The chat bot web application
- `/chat_bot_requirements.md` - Requirements for the chat bot integration
- `/todo.md` - Project task list and progress tracking

## MCP Server

The MCP server is built using Node.js and Express, providing a REST API for contact information lookup. It stores contact data in a simple JSON object for demonstration purposes.

### Features

- REST API endpoints for contact lookup
- Returns name, LinkedIn profile, email, and address for a given phone number
- Simple JSON-based data storage
- Error handling for non-existent contacts

### API Endpoints

- `GET /` - Root endpoint with API documentation
- `GET /api/contact/:phoneNumber` - Get contact information for a specific phone number
- `GET /api/contacts` - Get all available contacts

## Chat Bot Web Application

The chat bot web application provides a user-friendly interface for querying contact information from the MCP server.

### Features

- Clean, modern user interface
- Real-time contact information lookup
- Displays contact details in a formatted card
- Handles error cases gracefully
- Responsive design for mobile and desktop

## Setup and Installation

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### MCP Server Setup

1. Navigate to the MCP server directory:
   ```
   cd mcp_server
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the server:
   ```
   npm start
   ```

4. The server will run on port 3000 by default (http://localhost:3000)

### Chat Bot Web App Setup

1. Navigate to the web app directory:
   ```
   cd web_app
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the web app:
   ```
   npm start
   ```

4. The web app will run on port 8080 by default (http://localhost:8080)

## Usage

1. Start both the MCP server and the chat bot web app
2. Open the chat bot web app in your browser (http://localhost:8080)
3. Enter a phone number in the format `+12025550123` to look up contact information
4. The chat bot will display the contact details if found

## Sample Phone Numbers

The following sample phone numbers are available for testing:

- `+12025550123` - John Smith
- `+14155550189` - Sarah Johnson
- `+16175550156` - Michael Chen
- `+19175550178` - Emily Davis
- `+13105550192` - David Wilson

## License

This project is licensed under the ISC License.
