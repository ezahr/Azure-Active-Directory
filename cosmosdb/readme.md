

[create-notebook-visualize-data](https://docs.microsoft.com/nl-nl/azure/cosmos-db/create-notebook-visualize-data)

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


