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
![dotnet new command options](https://github.com/nagasudhirpulla/pluralsight_csharp_fundamentals_notes/raw/master/assets/dotnet_new_options.png)
