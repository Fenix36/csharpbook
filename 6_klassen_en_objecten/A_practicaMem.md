# Bookmark Manager
Maak een "bookmark manager". Deze tool zal in de console aan de gebruiker 5 favoriete sites vragen: naam en url. Vervolgens zal de tool alle sites in een lijst tonen met een nummer voor. De gebruiker kan dan de nummer intypen en de tool zal automatisch de site in de browser openen. 

Je opdracht:

1. Maak een array waarin je 5 bookmark objecten kan plaatsen. 
2. Vul de applicatie aan zodat de gebruiker: een bestaand bookmark kan verwijderen en een bestaand bookmark kan aanpassen

Enkele zaken die je nodig hebt:

**BookMark klasse:**
```csharp
class BookMark
{

    public string Naam { get; set; }
    public string URL { get; set; }
    public void OpenSite()
    {
        Process.Start("Iexplore.exe", URL);
    }
}
```
**Voorbeeld van hoe de bookmark klasse zal werken:** 
```csharp
BookMark u = new BookMark();
u.Naam = "Windows";
u.URL = "www.google.be";
u.OpenSite();
```

