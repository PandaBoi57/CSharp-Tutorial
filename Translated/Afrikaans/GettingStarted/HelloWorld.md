# Om te begin:

## Hello Werld

As jy ooit 'n programmerings taal geleer het, sal jy weet, die eerste program wat jy sal skryf gewoonlik genoem word "Hello, world", of eerder "Goeie More, Suid Afrika", en wie is ons om daai tradisie te verbreek? Gebruik "Visual Studio Community (voorgestel in die vorige hoofstuk), en kies "**File** -> **New** -> **Project**" van die projek dialoog. Kies dan "Console App (.NET framework)". Hierdie is die heel basiese program tipe vir die "Windows" stelsel, maar dit is 'n goeie plek om te begin leer. Nadat jy "OK" gedruk het sal "Visual Studio" 'n nuwe projek vir jou oopmaak, met 'n lêer met die naam van "Program.cs" ingesluit. Nou begin die pret, dit behoort so te lyk:

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

As mens mooi kyk lyk dit nie eintlik asof daar iets gebeur nie. Probeer om die program te hardloop deur die F5 sleutel te druk. Visual Studio sal jou bronkode saamstel (English Compile) en dit dan uitvoer. Soos jy kan sien is daar nie baie wat gebeur nie. Al wat gebeur is dat 'n swart venster op die skerm flits en dan verdwyn. Die rede hiervoor is dat op hierdie stadium doen die program eintlik niks nie. In die volgende hoofstuk sal ons hierdie lyne bronkode deurgaan en sien wat hulle doen, maar vir nou eers sal dit lekker wees as ons iets op die skerm kan sien. So kom ons gee voor asof ons slim is en alles weet wat daar te wete is van C# af ,en voeg 'n paar lyne bronkode by sodat daar iets op die skerm kan verskyn. Tussen die laaste stel krulhakies "{}" voeg die volgende lyne bronkode by (Jy is welkom om "Hello World!" te vervang met "Goeie More, Suid Afrika!"):.

```cs
Console.WriteLine("Hello, world!");
Console.ReadLine();
```

Jou eerste program se bron kode behoort so te lyk:

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

Druk weer die F5 sleutel om die program te hardloop, hierdie keer sal die swart venster oop bly, en "Hello World!" of "Goeie More, Suid Afrika!" vertoon. So ons het twee lyne bygevoeg, maar wat doen hulle? Een van die lekker dinge van C# en .NET is dat baie van die bron kode ooglopend sin maak, selfs vir diegene sonder die nodige kennis van die taal, soos die voorbeeld uitwys.

Die eerste lyn maak gebruik van die "Console class" om 'n lyn teks te wys, die tweede lyn lees 'n lyn teks van die konsole. Lees? Hoekom? Eintlik is dit 'n bietjie van 'n truuk, want sonder dit sal die program die eerste lyn wys en onmiddelik die venster weer toe maak voor jy die lyn teks kan sien.

Die "Readline" bevel maak dat die program oop bly en vir jou wag om iets te doen. Jy sal ook sien dat die program toelaat dat jy iets in die oop venster kan tik. Jy kan die venster toemaak deur die "Enter" knoppie te druk. Veels geluk, jy het so pas jou eerste C# program geskryf. Lees meer in die volgende hoofstuk oor hoe die program eintlik werk.