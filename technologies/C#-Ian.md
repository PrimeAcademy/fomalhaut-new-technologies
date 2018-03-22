# C# Example by Ian Robertson for Demonstration Purposes

## About
C# is a simple, easy to use, type-safe object oriented programming language that uses the .NET framework. C# is highly used in game development.  

## Set Up
To get started with C#, you must install "c#" on visual studio code and ".NET Core SDK" ![.NET Core SDK](https://www.microsoft.com/net/download/macos) to your computer. Once installed enter the following in your console to create a new project. 

`dotnet new console -o myApp`

## Hello World
1. Navigate to the program.cs file and enter the following code

`   using System;
    using System.Collections.Generic;
    using System.Linq;

    namespace myApp
    {
        class Program
        {
            static void Main(string[] args)
            {
                var name = ", Ian";
                Console.WriteLine($"Hello{name}!");
            }
        }
    }
`

## Next steps
The next steps for C# would be to figure out how to begin seeing code on the DOM and building out practice applications to learn more about the .NET Framework as well as C# itself. 