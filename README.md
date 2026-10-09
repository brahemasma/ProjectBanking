# 🏦 ProjectBanking

## 📌 Overview

**ProjectBanking** is a banking management application designed to provide secure APIs for managing clients, agents, branches, and banking transactions.

The project follows a layered architecture to ensure maintainability, scalability, and separation of concerns.

## 🛠️ Technologies

### Backend

* ASP.NET Core Web API
* C#
* Entity Framework Core
* SQL Server
* JWT Authentication
* RESTful APIs

### Frontend

* Angular
* TypeScript
* HTML5 / CSS3
* RxJS

## ✨ Features

* 🔐 User authentication with JWT
* 👥 Client management (Create, Read, Update, Delete)
* 🏢 Bank branch management
* 👨‍💼 Agent management
* 💳 Banking transaction management
* 🔎 Client search
* 🛡️ Secured API endpoints using authorization
* 🔗 Frontend and backend integration

## 📂 Project Structure

```text
ProjectBanking/
├── Bank.Api/
│   ├── Controllers/
│   ├── DTOs/
│   │   ├── Auth/
│   │   └── Clients/
│   ├── Services/
│   ├── Models/
│   ├── Data/
│   ├── Program.cs
│   └── appsettings.json
│
├── bank.front/
│   ├── src/
│   ├── public/
│   ├── angular.json
│   └── package.json
│
└── README.md
```

*Note: Update the folder names and structure to match your actual repository.*

## ⚙️ Prerequisites

Before running the project, make sure you have installed:

* .NET SDK
* Node.js and npm
* Angular CLI
* SQL Server
* Visual Studio or Visual Studio Code

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd ProjectBanking
```

### 2. Configure the database

Update the connection string in `appsettings.json`.

Configure Entity Framework Core and apply the database migrations if required.

```bash
dotnet ef database update
```

### 3. Run the backend

```bash
cd Bank.Api
dotnet restore
dotnet run
```

### 4. Run the frontend

Open a new terminal:

```bash
cd bank.front
npm install
ng serve
```

Open the local Angular URL displayed in the terminal.

## 🔒 Authentication

The application uses JSON Web Tokens (JWT) to authenticate users and protect secured API endpoints.

Include the following header in requests to protected endpoints:

```http
Authorization: Bearer <YOUR_JWT_TOKEN>
```

## 🔌 API Endpoints

| Method | Endpoint              | Description          |
| ------ | --------------------- | -------------------- |
| POST   | `/api/auth/login`     | Authenticate a user  |
| GET    | `/api/clients`        | Retrieve all clients |
| GET    | `/api/clients/{id}`   | Retrieve a client    |
| POST   | `/api/clients`        | Create a client      |
| GET    | `/api/clients/search` | Search for clients   |

*These endpoints are indicative; adjust them to match your controller routes.*

## 🌿 Git Workflow

The project can be organized into separate branches for backend and frontend development:

* `main` — stable version
* `develop` — integration branch
* `backend` — backend development
* `frontend` — frontend development

## 👩‍💻 Development

Contributions and improvements are welcome. Follow the existing project structure and coding conventions when adding new features.

## 📄 License

This project is intended for educational and development purposes unless otherwise specified.
# ProjectBanking
