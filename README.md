# Use a database with minimal API, Entity Framework Core, and ASP.NET Core

# Learning objectives
1. Learn how to add Entity Framework Core to a minimal API application.
2. Persist data to an in-memory datastore.
3. Persist data to a SQLite database.

# Understand EF Core
EF Core is a lightweight, extensible, open source, and cross-platform data access technology for .NET applications.

EF Core can serve as an object-relational mapper, which:

Enables .NET developers to work with a database by using .NET objects.
Eliminates the need for most of the data-access code that typically needs to be written.
EF Core supports a large number of popular databases, including SQLite, MySQL, PostgreSQL, Oracle, and Microsoft SQL Server.

# The model
With EF Core, data access is performed by using a model. A model is made up of entity classes and a context object that represents a session with the database. The context object allows querying and saving data.

# The context class
This application has only one entity class, but most applications have multiple entity classes. The context class is responsible for querying and saving data to your entity classes, and for creating and managing the database connection.

# Use the EF Core in-memory database
EF Core includes an in-memory database provider that can be used to test your application. The in-memory database provider is useful for testing and development, but it shouldn't be used in production. In the next unit, you'll use the in-memory database provider to create a database and perform CRUD operations on it.

# Steps to add a new database provider
1. Add one or more NuGet packages to your project to include the database provider.
2. Configure the database connection.
3. Configure the database provider in the ASP.NET Core services.
4. Perform database migrations.
