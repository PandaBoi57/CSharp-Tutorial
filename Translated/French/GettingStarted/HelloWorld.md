# Guide de démarrage:

## Hello, world!

Si vous vous êtes déjà formé à un langage de programmation, vous savez qu'on commence toujours par l'exemple "Hello, world!", et qui sommes-nous pour briser une si belle tradition? Lancer Visual Studio Community (introduit dans le chapitre précédent) et choisissez **Fichier** -> **Nouveau** -> **Projet**. Dans la fenêtre de création de projet, choisissez une Application Console (Framework .NET). Il s'agit du type d'application le plus basique sur un système Windows, mais c'est un bon outil pour apprendre le langage C#. Lorsque vous cliquez sur OK, Visual Studio vous crée un nouveau projet incluant un fichier nommé Program.cs. C'est là que tout se passe et ça ressemble à quelque chose comme ça:

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

En réalité, toutes ces lignes n'accomplissent rien, en tout cas n'en donnent pas l'impression. Essayer de lancer l'application en appuyant sur la touche F5 de votre clavier. Visual Studio déclenche la compilation et l'exécution de votre code mais, comme vous le constaterez, il ne se passe pas grand chose. Vous apercevrez peut-être une fenêtre noire s'ouvrir et se fermer aussitôt. Ceci se produit car notre application ne faire encore rien. Dans le prochain chapitre, nous passerons ces lignes en revue pour comprendre leur rôle mais, pour l'instant, nous voudrions voir un premier résultat donc faites comme si vous saviez tout à propos de C# et ajoutez deux lignes de code pour afficher quelque chose. A l'intérieur du dernier bloc de { }, ajoutez ces lignes :

```cs
Console.WriteLine("Hello, world!");
Console.ReadLine();
```

Le code de votre première application devrait ressembler à ceci :

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

A nouveau, appuyez sur F5 pour la lancer et vous verrez que la fenêtre noire reste maintenant visible et affiche même nos salutations au monde. Très bien, nous avons ajouté deux lignes de code, mais que font-elles ? Un des aspects sympa de C# et du Framework .NET est que beaucoup de code est compréhensible même pour les non initiés, ce que montre cet exemple.

La première ligne utilise la classe Console pour afficher une ligne de texte, et la seconde lit une ligne de texte depuis la console. Lit ? Pourquoi ? En fait, c'est d'une sorte d'astuce sans laquelle l'application se terminerait et fermerait la fenêtre contenant la ligne affichée avant que quiconque ait eu le temps de la lire.

L'instruction ReadLine demande à l'application d'attendre une action de l'utilisateur et, comme vous le constaterez, la fenêtre console vous permet maintenant de saisir du texte. Appuyez sur Entrée pour la fermer. Félicitations, vous venez juste de créer votre première application C# ! Lisez la suite dans le chapitre suivant pour plus d'informations sur ce qui se passe réellement.