# Contact List
A simple practice WEB API project built on .NET Core 3.1.

## Summary
this application will only meet the below use case.

- List contacts
- Add a contact
- Edit contact
- Delete/Inactivate a contact

## (No Authentication provided, No logging provided (That doesn't mean I am not aware of such stuff)

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
 7. Call AddContact API first to save some records.
 8. In case of error please check connection of databse and entity framework core
