# Meeting-Management-System

This is a .NET Core-based Meeting Management System that allows users to schedule, manage, and view meetings. The system supports public and private meetings, with different functionalities for logged-in and guest users.

## Features

1. **Home Page**
   - Displays public meetings, accessible without logging in.
   - Lists upcoming and past meetings with details such as title, date and time, duration, author, and location.
   - Includes a "View Details" button for each meeting, which shows the meeting description.
   - Option to log in or register from the home page.

2. **User Dashboard (After Logging In)**
   - Navigation bar includes:
     - **Meets:** Displays public meetings.
     - **My Meets:** Shows meetings created by the logged-in user, including upcoming and past meetings.
     - **Create Meets:** Provides a form for creating new meetings.
     - **Hello [username]:** Links to the user profile page, where account details can be modified.
     - **Logoff:** Logs the user out.

3. **Create Meet**
   - Form fields include:
     - Title
     - Date and Time
     - Duration (e.g., 01:00 hours)
     - Description
     - Location
     - "Is Public?" checkbox to mark the meeting as public or private.

4. **User Profile**
   - Allows users to update account details, change their password, and manage external logins.
   - Supports password updates and displays two-factor authentication settings.

## Prerequisites

- .NET Core SDK installed
- SQL Server for database management

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Dishatimbadiya/Meeting-Management-System
   ```

2. **Database Configuration**

Update the connection string in appsettings.json to point to your SQL Server instance.

3. **Run the Application**

  ```bash
  dotnet build
  dotnet run
  ```
  The application will be accessible at http://localhost:5000 by default.

4.  **Database Migrations (if applicable)**
   ```bash
    dotnet ef database update
  ```

## Usage
### Public Meetings: 
  - View upcoming and past public meetings without logging in.
  - User Registration and Login: Create an account or log in to access additional features.
  - Create Meetings: Fill out the form to schedule new meetings, marking them as public or private.
  - Manage Meetings: View and edit your created meetings under "My Meets."

## Technologies Used
  - .NET Core
  - Entity Framework Core
  - SQL Server
  - ASP.NET MVC


