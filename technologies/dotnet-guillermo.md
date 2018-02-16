# .NET Example by Guillermo Olivos

## About
.NET is a Microsoft based free, cross platform, open source developer platform for building many different types of applications.”

C# and VB.NET (among others) all compile to the same intermediate language (IL), which runs against the same .NET Framework runtime libraries. So in other words, .NET is many things, but this is an example of using .NET writing in C#.

## Set Up
To get started with .NET, you must install a .NET compiler on your MacOS. You can get started in 10 minutes by following the instructions found here:

https://www.microsoft.com/net/learn/get-started/macos

1) Download and install the .NET SDK (Software Development Kit)

2) Open a new command prompt and run the following commands.

dotnet new console -o myApp
cd myApp

The dotnet command will create a new application of type console for you. The -o parameter will create a directory named myApp where your app will be stored, and populates it with the required files. The cd myApp command puts you into the newly created app directory.

The main file in the myApp folder is Program.cs. By default, it already contains the necessary code to write "Hello World!" to the Console (which is helpful for the purposes of this assignment.)

3) In your command prompt, run the following command:

dotnet run
Congratulations, you've built and run your first .NET app!




## Hello World

Here is a link to my [Hello World]https://github.com/gcolivos/basic-dotnet-csharp example built with .NET and C#. It's straight from the Microsoft website and has a console.log of [Hello World] along with some arrays with add and loop functionality.

## Next steps

The next steps for learning this is to go deeper into the relationships amongst the different members of the .NET family. There are many additional tutorials available I'd be excited to dive into!