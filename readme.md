# Contoso University (Microsoft ASP.NET Core 3)

## Prerequisites

* [Visual Studio 2019](https://visualstudio.microsoft.com/downloads/) with the ASP.NET and web development workload (the Community edition is sufficient)
* [.NET Core 3.0 SDK or later](https://dotnet.microsoft.com/download/dotnet-core/3.0)

## Database engines

These instructions use [SQL Server LocalDB](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/sql-server-2016-express-localdb), a version of SQL Server Express that runs only on Windows.

## The App

The app is a basic university web site. Users can view and update student, course, and instructor information. Here are a few of the screens:

![Students Index page](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro/_static/students-index30.png)

![Students Edit page](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro/_static/student-edit30.png)

To run the app after downloading the solution:

* Build the project.
* In Package Manager Console (PMC) run the following command:

  ```powershell
  Update-Database
  ```

* Run the project (Debug -> Start new instance) to seed the database and open the site in your default web browser.

* At any time you need to return the database to the default state, stop the app and run the following commands:

  ```powershell
  Drop-Database
  Update-Database
  ```

More information is available from the Microsoft ASP.NET Docs site at the [Razor Pages with Entity Framework Core in ASP.NET Core - Tutorial](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-3.1&tabs=visual-studio).