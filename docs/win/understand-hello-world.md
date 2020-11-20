# Understanding Hello World

Last lesson, you created your Hello World project:

```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hello world!");
        }
    }
}
```

So what does this code really mean? Let's find out!

## using System

```csharp
using System;
```

This line means we can use all classes in the [System][1] namespace without fully qualifing it. (Typing `System.` before it)

[1]: https://docs.microsoft.com/en-us/dotnet/api/system?view=dotnet-plat-ext-5.0

## namespace HelloWorld

This isn't required, but when you're making a library, you should use it so there won't be any name conflicts. Examples:

* `System`
* `System.Linq`
* `System.Text`
* `System.Collections.Generic`

Your class goes in the required braces.

## class Program

All of your code goes inside a method, which has to be in a class. (Actually, you don't in C# 9, but when making more complex things, you shouldn't use this.) Like namespaces, methods, fields, events, and properties go inside the braces.

## static void Main()

If you want to run your code, you have to have a main function. Let's break this down.

### static

`static` means you don't have to have a Program, you can just call it. This is required for Main.

### void

`void` means Main doesn't return, or pass any information. You can return an int, the exit code, but we won't here.

### Main

`Main` is the name of the function. Case matters.

### The parentheses

Main takes no arguments with nothing in between. When using the command line, you can pass arguments. Remember the time we removed `string[] args`? That is a parameter.

### Console.WriteLine("Hello world!")

Console.WriteLine is the function to print. You put something inside the parentheses, here it's a string. Strings, or text, have to be inside quotes. Every statement ends with a semicolon. (;)
