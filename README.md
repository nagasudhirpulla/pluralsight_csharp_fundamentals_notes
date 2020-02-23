# pluralsight_csharp_fundamentals_notes
This is the notes for pluralsight c# fundamentals course by Scott Allen - https://www.pluralsight.com/courses/csharp-fundamentals-dev

## Motivation
- .NET Core framework can be used to produce apps
- C# language is used to express / control the framework to produce the desired apps using the framework

## Install .NET Core SDK
https://dotnet.microsoft.com/download

## Install Visual Studio Code
https://code.visualstudio.com/download

## .NET and .NET Core Frameworks
![.NET and .NET Core Frameworks](https://github.com/nagasudhirpulla/pluralsight_csharp_fundamentals_notes/raw/master/assets/net_and_core_diffs.png)

## .NET Components
- .NET mainly contains .NET CLR (Common Language Runtime) and .NET FCL (Framework Class Library).
- CLR understands C#, manages memory and executes C# programs on .NET framework
- FCL contains libraries to perform common tasks like HTTP requests, message encryption etc.

![.NET Runtime and Framework Class Library (FCL)](https://github.com/nagasudhirpulla/pluralsight_csharp_fundamentals_notes/raw/master/assets/dotnet_components.png)

## .NET Core command line
dotnet CLI (command line interface) can be used in the command prompt (cmd)
- dotnet versions and other info ```dotnet --info```
- Use **--help** for help on any command ```dotnet new --help```

## Creating .NET Core project using dotnet new command
- Use ```dotnet new console``` to create a console app project
- Use ```dotnet new mvc``` to create a mvc web app project
- Use ```dotnet new webapp``` to create a razor pages web app project

![dotnet new command options](https://github.com/nagasudhirpulla/pluralsight_csharp_fundamentals_notes/raw/master/assets/dotnet_new_options.png)

## Create a console app in .NET Core
```dotnet new console```
- This command will create a new console app in .NET Core
- We will get a **.csproj** file that contains project info and a **Program.cs** file that contains the C# code
- .csproj file is shown below that has information about the console application frameworks configuration
```xml
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>netcoreapp3.1</TargetFramework>
  </PropertyGroup>
</Project>
```
- .cs file is shown below that contains **static void Main** function that serves as an entry point for the console app
```cs
using System;
namespace console_app
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

## Running the console app
- The console app can be run using the command ```dotnet run```
- This command will build and run the console app
