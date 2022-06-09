Liam's note.

0. Create project. Check Use controller (Uncheck to use minimal APIs)

1. Strip Weatherforacast from Program.cs (or don't bother)

2. Add Dependencies Packages 

3. Install dotnet tool

View > Other Windows > Package Manager Console
PM> dotnet tool install --global dotnet-ef
PM> dotnet ef 

4. Download and install: Sql Server & SqlServer Management Studio (SSMS)

5. Add Superhero model class

6. Create folder Data, and Add DataContext.cs
 
7. Update ConnectionStrings in appsettings.json

8. Add controller. 
Right click on COntrollers folder
Add > Controller 
Controller > API > API Controller - Empty
Name> SuperHeroController.cs

9. Add CRUD operation codes in SuperHeroController.cs

10. Add service injection in Program.cs

11. Run migration
In Package Manager Console, PM> dotnet ef to see command options for the migration
PM> cd .\SuperHeroAPI
PM> dotnet ef migrations add CreateInitial
--> this creates migration file called xxxx_CreateInitial.cs

12. Update Database
PM> dotnet ef database update
--> Open SqlServer Management Studio and see the new database 
and table have been created.

11. Add CRUD operation codes in Program.cs

12. Run swagger UI to test all CRUD operations and check SqlServer for the actual data

Tutorial at
https://www.youtube.com/watch?v=Fbf_ua2t6v4

Github at
https://github.com/patrickgod/SuperHeroAPI-DotNet6



