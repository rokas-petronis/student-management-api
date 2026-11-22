# Student Administration Web Project

A learning project built with **ASP.NET Core (.NET 8)** that explores building a web API, connecting it to a SQL Server database, and displaying student information in a simple HTML/JavaScript frontend.

The project was created to practice backend development, Entity Framework Core, authentication, and communication between a browser and an API.

## Features

- **Student and grade data:** Entity Framework Core models for students and their grades.
- **Student API:** Includes a student-data endpoint used by the frontend (`GET /api/School/Students`).
- **Database integration:** Uses Microsoft SQL Server and Entity Framework Core for data access.
- **Authentication setup:** ASP.NET Core Identity endpoints for account registration and login.
- **Swagger:** Interactive API documentation in the development environment, with bearer-token configuration.
- **Basic frontend:** HTML, CSS and JavaScript page that requests student data from the API and displays names.
- **Sample records:** The application attempts to add example students and grades when the students table is empty.

## Technologies

- C# / .NET 8
- ASP.NET Core Web API
- Entity Framework Core
- Microsoft SQL Server
- ASP.NET Core Identity
- Swagger / OpenAPI
- HTML, CSS and JavaScript

## Running locally

### Requirements

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- Microsoft SQL Server

Clone the repository:

```bash
git clone https://github.com/rokas-petronis/web-project.git
cd student-management-api
```

The project currently contains a **machine-specific SQL Server connection string** in `Program.cs` and `SchoolContext.cs`. To use a different computer, the database connection needs to be configured for an available SQL Server instance and a compatible database schema must exist. The frontend also uses a fixed local HTTPS API address.

Once the local database setup is available, start the application:

```bash
dotnet run --project web-project.csproj
```

In the development environment, Swagger UI is available at `/swagger` on the application's local URL. The static frontend is served from `wwwroot`.

## Project status

This is an educational project demonstrating selected backend and frontend concepts, **not a complete student administration system**. Some application functionality is experimental or unfinished.
