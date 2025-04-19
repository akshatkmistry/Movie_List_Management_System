# 🎬 Movie List Management System

A simple ASP.NET Web Forms application for tracking movies you've watched or want to watch. This college mini-project demonstrates basic web development concepts using ASP.NET, ADO.NET and SQL Server.

## Features

- User registration and login system
- Add, edit, and delete movies
- Track movie details (title, director, release year, genre)
- Mark movies as watched, unwatched, or plan to watch
- Rate movies on a scale of 1-5
- Dashboard with statistics about your movie collection
- Filter functionality by Watch Status

## Technologies Used

- ASP.NET Web Forms (.aspx, .aspx.cs)
- ADO.NET (for SQL Server communication)
- SQL Server (local DB with `Users` and `Movies` tables)
- HTML/CSS/JS (for styling and basic interactivity)
- Visual Studio 2022

## ⚙️ Setup Instructions

### 📦 Step 1: Initialize SQL Server Database

1. Open **SQL Server Management Studio** or any SQL client.
2. Run the SQL script located at: `App_Data/MovieTrackerDB.sql`

This will create the `MovieTrackerDB` database along with `Users` and `Movies` tables, and insert sample data.


### 🔧 Step 2: Update the Connection String

Ensure your connection string matches your SQL Server setup.

Update **both** of the following files:
- `Web.config`
- `App_Data/DatabaseConnection.cs`

### ▶️ Running the Application

1. Open the solution in Visual Studio 2022
2. Build the solution (this will restore NuGet packages)
3. Make sure your SQL Server service is running.
4. Press F5 or click the Run button to start the application
5. The application will open in your default web browser

### 🔐 Default Login

The database script creates two sample users:
- Username: admin, Password: admin123
- Username: user1, Password: user123

##  Project Structure

- **Login.aspx**: User authentication page
- **Register.aspx**: New user registration
- **Default.aspx**: Dashboard and movie listing
- **AddMovie.aspx**: Form to add new movies
- **EditMovie.aspx**: Form to edit existing movies
- **App_Data/DatabaseConnection.cs**: Database connection and query methods
- **App_Data/MovieTrackerDB.sql**: Database creation script

## Learning Outcomes

This project demonstrates:
- Creating a web application with ASP.NET Web Forms
- Implementing user authentication
- Database CRUD operations using ADO.NET
- Form validation and data handling
- Responsive UI design with Bootstrap
- Session management
