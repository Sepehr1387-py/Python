# C#
Console.WriteLine("Wählen Sie Ihren Aktivitätsfaktor:");
Console.WriteLine("1 = wenig aktiv (1,2)");
Console.WriteLine("2 = leicht aktiv (1,375)");
Console.WriteLine("3 = moderat aktiv (1,55)");
Console.WriteLine("4 = sehr aktiv (1,725)");

string auswahl = Console.ReadLine();

double faktor;

switch (auswahl)
{
    case "1":
        faktor = 1.2;
        break;

    case "2":
        faktor = 1.375;
        break;

    case "3":
        faktor = 1.55;
        break;

    case "4":
        faktor = 1.725;
        break;

    default:
        Console.WriteLine("Ungültige Auswahl.");
        Console.ReadKey();
        return;
}

double kalorienbedarf = 2250 * faktor;

Console.WriteLine("Ihr Kalorienbedarf beträgt "
                  + kalorienbedarf + " Kalorien.");

Console.ReadKey();
