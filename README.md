* Create new web api project - dotnet new webapi -o project_name
* Run project - dotnet run
* Build project - dotnet build
* Check version - dotnet --version
* List of dotnet sdks installed - dotnet --list-sdks

  docker command to run sql server container - 
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Vishal123' -p 1433:1433 --name sql1 -d mcr.microsoft.com/mssql/server:2022-latest

  When you’ve changed your data model (like adding a new entity class or modifying a property) and created a migration with:
  * dotnet ef migrations add <MigrationName>
  
  that migration only generates the code describing the changes — it doesn’t actually touch your database yet.

  To sync your actual database schema with those code changes, you run:
  * dotnet ef database update
 
That’s what applies all pending migrations to your database — creating tables, columns, relationships, indexes, etc.
