# 🚀 Leave Management System

![.NET](https://img.shields.io/badge/.NET-8-purple)
![ASP.NET](https://img.shields.io/badge/ASP.NET-Core-blue)
![Database](https://img.shields.io/badge/Database-SQLServer-red)
![License](https://img.shields.io/badge/License-MIT-green)

A simple **Leave Management Web Application** built using **ASP.NET Core, Entity Framework Core, and SQL Server**.

The system allows employees to submit leave requests and view leave records through a dashboard.

---

# 📌 Features

- Create leave requests
- View leave dashboard
- Automatic total leave day calculation
- SQL Server database integration
- REST API support
- Responsive UI with Bootstrap

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|--------|
| ASP.NET Core | Backend Framework |
| Entity Framework Core | ORM for database |
| SQL Server | Database |
| Razor Views | Frontend UI |
| Bootstrap | Styling |
| C# | Programming Language |

---

# 📂 Project Structure

```
leave-management/
│
├── Controllers
│   └── LeaveController.cs
│
├── Models
│   └── LeaveRecordes.cs
│
├── Data
│   └── AppDbContext.cs
│
├── Views
│   └── Leave/
│
├── wwwroot/
│
├── Program.cs
├── appsettings.json
└── README.md
```

---

# ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/leave-management.git
cd leave-management
```

### 2️⃣ Install Requirements

Make sure you have installed:

- .NET 8 SDK
- SQL Server
- Visual Studio 2022 or VS Code

Install Entity Framework CLI if needed:

```bash
dotnet tool install --global dotnet-ef
```

---

# 🗄️ Configuration

Open **appsettings.json** and update the database connection string:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=LeaveManagementDB;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

---

# 🧱 Database Setup

### Create Migration

```bash
dotnet ef migrations add InitialCreate
```

### Apply Migration

```bash
dotnet ef database update
```

This will create the **LeaveManagementDB** database automatically.

---

# ▶️ Running the Application

Run the application using:

```bash
dotnet run
```

Or press **F5** in Visual Studio.

The application will start at:

```
https://localhost:xxxx
```

---

# 🔌 API Endpoints

| Method | Endpoint | Description |
|------|------|------|
| GET | /api/Leave/GetUserDetails | Get all leave records |
| POST | /api/Leave/AddLeave | Create leave request |

---

# 📦 Example Request

### Create Leave Request

```http
POST /api/Leave/AddLeave
Content-Type: application/json
```

```json
{
  "employeeName": "John",
  "leaveType": "Casual",
  "startDate": "2026-03-20",
  "endDate": "2026-03-22"
}
```

---

# 🚧 Future Improvements

- Authentication (JWT / Identity)
- Admin Leave Approval
- Email Notifications
- Leave Calendar
- Analytics Dashboard

---

# 👨‍💻 Author

**Binura Navodh**

---

⭐ If you like this project, consider giving it a **star on GitHub**.
