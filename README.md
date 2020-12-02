# Contact List
A simple practice WEB API project built on .NET Core 3.1.

## Summary
Implemented following things in the project
- User authentication through JWT Token
- Autofac container to implement dependency injection
- Serilog to log information and errors
- xUnit to write unit test cases for ContactsController.cs (Only limited scope covered)
- Entity Framework Core

this application will only meet the below use case.
- Authenticate user
- List contacts
- Add a contact
- Edit contact
- Delete/Inactivate a contact

## Prerequisite
 1. Dot Net Core 3.1
 2. Visual Studio 2019
 3. SQL Server 2014
 4. Postman tool (to test web api)

## Basic flows of events:
 
 1. Create table by using script 'CreateTableScript.sql', (Please change database name in script)
	Please change Connection strings mentioned in 'appsettings.json' as per your SQL DB credentials
	"ConnectionStrings": {
							"TestDBConnection": "Server=SERVER_NAME;Database=Test;Integrated Security=True;"
						},
 
 2. Go to solution directory (i.e. ManageContacts.sln) in visual studio command prompt
 3. enter command 'dotnet restore'
 4. enter command 'dotnet build'
 5. enter command 'dotnet run'
 6. import attached rest api collection file in postman i.e. 'Rest API Contacts.postman_collection.json'
 7. Call Authenticate API first then paste token in other api's authorization tab
 8. Call AddContact API first to save some records.
 9. In case of error please check connection of databse and entity framework core
 10. In case of Unauthorized response try to call authenticate api and then paste token in postman > authorization > select type as 'Bearer Token' > Then paste it. You will be authorized user then.
