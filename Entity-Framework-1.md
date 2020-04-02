## EF Core

### Tutorial Overview

- Build off a web app
- Build cshtml content to purpose
- Install db provider (NuGet)
- Create data Model
  - For each table, make a class in Models folder
  - Each class should have properties for each column
  - Properties and their corresponding columns should have the exact same names
  - Foreign keys should be stored as collections when made into properties
- Create database context
  - In Data folder, make a class for the database
  - DB class should have a property for each table, stored as `DbSet<TableName>` type
  - Create an override function to turn these classes into actual tables
  - Add this DbContext in Startup class
  - Ensure you are using the Data folder and the Microsoft Entity Framework Core in Startup
  - Add db url to app settings file
- You are now free to initialize the database and add data, from a specialized class
- Controller and Views can now be scaffolded (or built from scratch)
