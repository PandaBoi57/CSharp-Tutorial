# Getting started:

## Hello, world!

If you have ever learned a programming language, you know that they all start with the "Hello, world!" example, and who am I to break such a fine tradition? Start Visual Studio Community (introduced in the last tutorial), and select **File** -> **New** -> **Project**. From the project dialog, select the Console App (.NET framework). This is the most basic application type on a Windows system, but it's great for learning the language. Once you click Ok, Visual Studio creates a new project for you, including a file called Program.cs. This is where all the fun is, and it should look something like this:

```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    class Program
    {
        static void Main(string[] args)
        {
        }
    }
}
```

Actually, all these lines don't really accomplish anything, or at least it may seem so. Try running the application by pushing F5 on your keyboard. This will make Visual Studio compile and execute your code, but as you will see, it doesn't do that much. You will likely just see a black window launch and close again. That is because our application doesn't do anything yet. In the next chapter we will go through these lines to see what they are all about, but for now, we really would like to see some results, so let's pretend that we know all about C# and add a couple of lines to get some output. Inside the last set of { }, add these lines:

```cs
Console.WriteLine("Hello, world!");
Console.ReadLine();
```

The code of your first application should now look like this:

```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    class Program
    {
        static void Main(string[] args)
        {
                Console.WriteLine("Hello, world!");
                Console.ReadLine();
        }
    }
}
```

Once again, hit F5 to run it, and you will see the black window actually staying, and even displaying our greeting to the world. Okay, so we added two lines of code, but what do they do? One of the nice things about C# and the .NET framework is the fact that a lot of the code makes sense even to the untrained eye, which this example shows.

The first line uses the Console class to output a line of text, and the second one reads a line of text from the console. Read? Why? Actually this is a bit of a trick, since without it, the application would just end and close the window with the output before anyone could see it.

The ReadLine command tells that application to wait for input from the user, and as you will notice, the console window now allows you to enter text. Press Enter to close it. Congratulations, you have just created your first C# application! Read on in the next tutorial for even more information about what's actually going on.