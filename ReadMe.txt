dotnet --version
dotnet tool install --global dotnet-ef --version

dotnet ef -

add package manager

CMD+P and '>' and select package manager

dotnet ef database update -- this has created the sqllite database

open ctrl+p and > sqllite: Open DB and this should show the path of the databse, and click on it to open.

from the explorer we should be able to see the database.


dotnet new classlib -o Core -- Creates a new class library named Core


dotnet new classlib -o Infrastructure -- Creates a new class library named Core


dotnet sln add Core
dotnet sln add Infrastructure


:To add dependency from API to Infrastructure, cd to API:
dotnet add reference ../Infrastructure/ 

:To add dependency from Infrastructure to Core, cd to API:
dotnet add reference ../Core/ 

dotnet restore


//CORE is for Entities

//Infrastruc