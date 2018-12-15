# Getting started:

## Hello world explained

In the previous tutorial, we tried writing a piece of text to the console, in our first C# application. To see some actualy progress, we didn't go into much detail about the lies of code we used, so this tutorial is an explanation of the Hello world example code. As you can probably see from the code, some of the lines look similar, so we will bring them back in groups for an individual explanation. Let's start with the shortest and most common characters in our code: The `{` and `}`. They are often referred to as curly braces, and in C#, they mark the beginning and end of a logical block of code. The curly braces are used in lots of other languages, include C++, Java, JavaScript, and many others. As you can see in the code, they are used to wrap several lines of code which belong together. In later examples, it will be clearer how they are used.

Now, let's start from the beginning:

```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
```

**using** is a keyword, highlighted with blue by the editor. The using keyword imports a namespace, and a namespace is a collection of classes. Classes brings us some sort of functionality, and when working with an advanced IDE like Visual Studio, it will usually create parts of the trivial code for us. In this case, it created a class for us, and imported the namespaces which are required or expected to be used commonly. In this case, 5 namespaces are imported for us, each containing lots of useful classes. For instance, we use the Console class, which is a part of the System namespace.

On the other hand, we don't really use the *System.Linq* namespace yet (for example), so if you're a perfectionist, you may choose to remove this line, but it won't make much of a difference at this point.

As you can see, we even get our own namespace:

```cs
namespace ConsoleApp1
```

The namespace ConsoleApp1 is now the main namespace for this application and new classes will be a part of it by default. Obviously, you can change this, and create classes in another namespace. In that case, you will have to import this new namespace to use it in your appliation, with the using statement, like any other namespace.

Next, we define our class. Since C# is truly and Object Oriented language, every line of code that actually does something is wrapped inside a class. In this case, the class is simply called Program:

```cs
class Program
```

We can have more classes, even in the same file. For now, we only need one class. A class can contain several variables, properties, and methods, concepts we will go deeper into later. For now, all you need to know is that our current class only contains one method and nothing else. It's declared like this:

```cs
static void Main(string[] args)
```

This line is probably the most complicated one in this example, so let's split it up a bit. The first word is **static**. The static keyword tells us that this method should be accesible without instantiating the class, but more about this in our tutorial about classes.

The next keyword is **void**, and tells us what this method should return. For instance, it could be an integer or a string of text, but in this case, we don't want our method to return anything. (C# uses the keyword *void* to express the concept of *nothing*).

The next word is **Main**, which is simply the name of our method. This method is the so-called entry-point of our application, that is, the first piece of code to be executed, and in our example, the only piece to be executed.

Now, after the name of a method, a set of arguments can be specified within a set of parantheses. In our example, our method takes only one argument, called **args**. The type of the argument is a **string**, or to be more precise, an array of strings, but more on that later. If you think about it, this makes perfect sense, since Windows applications can always be called with an optional set of arguments. These arguments will be passed as text strings to our main method.

And that's it. You should now have a basic understanding of our first C# application, as well as the basic principles of what makes a console application work.

[Previous](HelloWorld.md)