# Leave Management System

## Description
The Leave Management System is a web application built using ASP.NET Core, Entity Framework Core, and SQL Server.
It allows employees to submit leave requests and view leave records through a dashboard.

---

## Features
- Create leave requests
- View leave dashboard
- Automatic total leave days calculation
- Store leave records in SQL Server database
- REST API integration
- Responsive UI using Bootstrap

---

## Technologies Used
- ASP.NET Core
- Entity Framework Core
- SQL Server
- Razor Views
- Bootstrap
- C#

---

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/leave-management.git
cd leave-management
## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/leave-management.git
cd leave-management
```

### 2. Install Dependencies

Make sure the following are installed on your system:

- .NET 8 SDK
- SQL Server
- Visual Studio 2022 or VS Code

Install Entity Framework CLI if it is not installed:

```bash
dotnet tool install --global dotnet-ef
```
## Configuration

Open **appsettings.json** and update the database connection string:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=LeaveManagementDB;Trusted_Connection=True;TrustServerCertificate=True;"
}
```
## Database Setup

### Create Migration

```bash
dotnet ef migrations add InitialCreate
```

### Update Database

```bash
dotnet ef database update
```

This will create the **LeaveManagementDB** database and required tables.
## Running the Application

Run the project using:

```bash
dotnet run
```

Or press **F5** in Visual Studio.

The application will start at:

```
https://localhost:xxxx
```
## API Endpoints

| Method | Endpoint | Description |
|------|------|------|
| GET | /api/Leave/GetUserDetails | Get all leave records |
| POST | /api/Leave/AddLeave | Create a leave request |
## Project Structure

```
leave-management/
│
├── Controllers
├── Models
├── Data
├── Views
├── wwwroot
│
├── Program.cs
├── appsettings.json
└── README.md
```
## Author

Binura Navodh


 
