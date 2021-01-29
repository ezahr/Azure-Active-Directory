

[create-notebook-visualize-data](https://docs.microsoft.com/nl-nl/azure/cosmos-db/create-notebook-visualize-data)

[pluralsight C#(https://app.pluralsight.com/course-player?clipId=13239d14-98fd-4ce8-88bd-f9ef8fc1f416)

## cd /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld

````
osxs-mbp:virtual-insanity osx$ mkdir helloworld
osxs-mbp:virtual-insanity osx$ cd helloworld/
osxs-mbp:helloworld osx$ mkdir src
osxs-mbp:helloworld osx$ mkdir test
osxs-mbp:helloworld osx$ cd src
osxs-mbp:src osx$ mkdir HelloWorld
osxs-mbp:src osx$ cd HelloWorld/
osxs-mbp:HelloWorld osx$ pwd
/Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld
`````
## dotnet new console
````
osxs-mbp:HelloWorld osx$ dotnet new console
The template "Console Application" was created successfully.

Processing post-creation actions...
Running 'dotnet restore' on /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld/HelloWorld.csproj...
  Determining projects to restore...
  Restored /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld/HelloWorld.csproj (in 179 ms).

Restore succeeded.

osxs-mbp:HelloWorld osx$ ls
HelloWorld.csproj	Program.cs		obj
osxs-mbp:HelloWorld osx$ 

````

## cd /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld
## dotnet add package Microsoft.Azure.Cosmos --version 3.16.0

https://www.nuget.org/packages/Microsoft.Azure.Cosmos/

## dotnet add package Microsoft.Extensions.Configuration.Json --version 5.0.0

https://www.nuget.org/packages/Microsoft.Extensions.Configuration.Json/


## /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld/HelloWorld.csproj
````
<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>netcoreapp3.1</TargetFramework>
  </PropertyGroup>

  <ItemGroup>
    <PackageReference Include="Microsoft.Azure.Cosmos" Version="3.16.0" />
    <PackageReference Include="Microsoft.Extensions.Configuration.Json" Version="5.0.0" />
  </ItemGroup>

</Project>

````

## /Users/osx/Projects/scratch/virtual-insanity/helloworld/src/HelloWorld/Program.cs

````
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}

````

|KEY|d[atabaseAccounts/cosmos-bdmcc/keys](https://portal.azure.com/#@boschpeteroutlook.onmicrosoft.com/resource/subscriptions/87d504e9-46e8-4b87-8f72-f207ee8e6dad/resourceGroups/cloud-shell-storage-westeurope/providers/Microsoft.DocumentDb/databaseAccounts/cosmos-bdmcc/keys) |
|--------|------------------------------------------------------------------|
|URI|https://cosmos-bdmcc.documents.azure.com:443/|
|primary key|kHUP25fn8kvWoIOVJTUJB9xqjSnHjzMMAOcavs50yOrdAO2ooJiQEIp2K5f1rYj2RiEoDzcEtuOwUViiCn33iQ==|
||AccountEndpoint=|https://cosmosbdmcc.documents.azure.com:443/;AccountKey=kHUP25fn8kvWoIOVJTUJB9xqjSnHjzMMAOcavs50yOrdAO2ooJiQEIp2K5f1rYj2RiEoDzcEtuOwUViiCn33iQ==;|
|SECONDARY KEY|Cq2nfhzzVJJvje8fcu6IxZ2LkDU7OzxC5bexrdzTj9J1gUPwfuDc43rLu5vns0ExEyGgJDGj0mkxNFGyAq4Oqw== |
|PRIMARY CONNECTION STRING| Cq2nfhzzVJJvje8fcu6IxZ2LkDU7OzxC5bexrdzTj9J1gUPwfuDc43rLu5vns0ExEyGgJDGj0mkxNFGyAq4Oqw==|
|SECONDARY CONNECTION STRING|AccountEndpoint=https://cosmos-bdmcc.documents.azure.com:443/;AccountKey=Cq2nfhzzVJJvje8fcu6IxZ2LkDU7OzxC5bexrdzTj9J1gUPwfuDc43rLu5vns0ExEyGgJDGj0mkxNFGyAq4Oqw==;   |


