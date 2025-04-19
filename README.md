# Movie Tracker Application

A simple ASP.NET Web Forms application for tracking movies you've watched or want to watch. This college mini-project demonstrates basic web development concepts using ASP.NET and MySQL.

## Features

- User registration and login system
- Add, edit, and delete movies
- Track movie details (title, director, release year, genre)
- Mark movies as watched, unwatched, or plan to watch
- Rate movies on a scale of 1-5
- Dashboard with statistics about your movie collection
- Search functionality to find specific movies

## Technologies Used

- ASP.NET Web Forms (C#)
- MySQL Database
- ADO.NET for database operations
- Bootstrap 5 for responsive UI

## Setup Instructions

### Prerequisites

- Visual Studio 2022
- MySQL Server installed and running
- MySQL Connector/NET (installed via NuGet)

### Database Setup

1. Open MySQL Workbench or any MySQL client
2. Run the SQL script located at `MovieTrackerApp/App_Data/MovieTrackerDB.sql`
3. This will create the database and required tables with sample data

### Connection String

The application is configured to connect to MySQL with these default settings:
- Server: localhost
- Database: MovieTrackerDB
- Username: root
- Password: password

If your MySQL setup is different, update the connection string in:
- `Web.config`
- `App_Data/DatabaseConnection.cs`

### Running the Application

1. Open the solution in Visual Studio 2022
2. Build the solution (this will restore NuGet packages)
3. Make sure MySQL is running
4. Press F5 or click the Run button to start the application
5. The application will open in your default web browser

### Default Login

The database script creates two sample users:
- Username: admin, Password: admin123
- Username: user1, Password: user123

## Project Structure

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