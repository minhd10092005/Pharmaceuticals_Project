# 💊 Pharmaceuticals Project

A Full-Stack Pharmaceutical Web Application built with **ASP.NET Core 10, React.js, and MySQL**.

This project aims to provide a web-based platform for browsing pharmaceutical products and managing product-related information. It demonstrates full-stack development skills, RESTful API integration, database management, and modern web application architecture.

---

## 📌 Project Overview

**Pharmaceuticals Project** is a full-stack web application designed to connect customers with pharmaceutical products through an intuitive web interface.

The application separates the frontend and backend into two independent components. The backend provides RESTful APIs to handle business logic and database operations, while the frontend delivers a responsive user interface and communicates with the backend through HTTP requests.

### Key Objectives

- Build a full-stack web application using modern technologies.
- Develop RESTful APIs for frontend and backend communication.
- Implement database connectivity and data management.
- Apply a structured backend architecture.
- Create a user-friendly interface for browsing pharmaceutical products.

## ✨ Main Features

### Customer Interface

- **Product Catalog:** Browse and explore available pharmaceutical products.
- **Product Details:** View detailed information about individual products.
- **Contact & Feedback:** Provide a way for customers to send inquiries and feedback.

### Authentication & Authorization

- User authentication using JSON Web Tokens (JWT).
- Role-based access for Admin and User.
- Protected functionality based on user permissions.

### Backend

- RESTful API development.
- Business logic separation.
- Database operations using Entity Framework Core.
- MySQL database integration.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, Vite, JavaScript, CSS |
| Backend | C#, ASP.NET Core 10, ASP.NET Core Web API |
| ORM | Entity Framework Core |
| Database | MySQL |
| Authentication | JWT (JSON Web Token) |
| API Communication | HTTP / RESTful API |
| Development Tools | Visual Studio, Visual Studio Code, MySQL Workbench, Git, GitHub |

## 🏗️ System Architecture

The application follows a Client–Server architecture with separate frontend and backend layers.

```text
       USER
         |
         v
  REACT.JS FRONTEND
      (Vite)
         |
         | HTTP Requests
         | RESTful API
         v
  ASP.NET CORE 10
      BACKEND
         |
    +----+-----+
    |          |
    v          v
 Controllers  Services
    |          |
    +----+-----+
         |
         v
  ENTITY FRAMEWORK CORE
         |
         v
      MYSQL
     DATABASE
```

### Architecture Description

- **Frontend:** Handles user interactions, page rendering, and API communication.
- **Backend:** Processes HTTP requests and manages application business logic.
- **Entity Framework Core:** Provides object-relational mapping (ORM) between application entities and database tables.
- **MySQL:** Stores application data and maintains relationships between entities.

## 📂 Project Structure

```text
Pharmaceuticals_Project/
│
├── Backend/
│   ├── Controllers/
│   ├── Services/
│   ├── Repositories/
│   ├── Models/
│   ├── Data/
│   └── ...
│
├── Frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── Pharmaceuticals_Project.sln
├── .gitignore
└── README.md
```

*Note: The directory structure above illustrates the main application layers. Refer to the source code for the complete implementation.*

## 🚀 Getting Started

Follow these instructions to run the project locally.

### Prerequisites

Make sure you have installed:

- [Visual Studio 2022](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)
- [Node.js](https://nodejs.org/)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

### 1. Clone the Repository

```bash
git clone https://github.com/minhd10092005/Pharmaceuticals_Project.git

cd Pharmaceuticals_Project
```

### 2. Configure the Database

1. Start your MySQL Server.
2. Open the backend project.
3. Configure the database connection string in `appsettings.json`.
4. Replace the database username and password with your local MySQL credentials.
5. Ensure the database and required tables are initialized according to the project's database configuration.

Example connection string:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Database=PharmaceuticalsDB;User=root;Password=YOUR_PASSWORD;"
  }
}
```

### 3. Run the Backend

Open a terminal:

```bash
cd Backend
dotnet restore
dotnet run
```

The backend is configured to run locally on:

- HTTPS: `https://localhost:7263`
- HTTP: `http://localhost:5298`

### 4. Run the Frontend

Open another terminal:

```bash
cd Frontend
npm install
npm run dev
```

The frontend is available at:

```text
http://localhost:5173
```

Make sure the frontend API configuration points to the correct backend URL.

## 🔐 Security Notes

- Do not commit database passwords, JWT secrets, or other sensitive configuration values.
- Use your own local configuration when running the application.
- Authentication tokens should be handled securely.
- Never upload production credentials to a public repository.

## 🎯 Skills Demonstrated

Through this project, I gained practical experience in:

- Full-stack web application development.
- Building RESTful APIs with ASP.NET Core.
- Developing frontend interfaces using React.js.
- Working with relational databases and MySQL.
- Integrating Entity Framework Core.
- Implementing JWT-based authentication and authorization.
- Connecting frontend applications with backend services.
- Using Git and GitHub for source code management.

## 👨‍💻 Author

**minhd10092005**

GitHub: [@minhd10092005](https://github.com/minhd10092005)

---

⭐ Thank you for taking the time to explore this project!
