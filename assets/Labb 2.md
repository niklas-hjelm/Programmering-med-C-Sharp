# Lab2 – Skapa en simpel butik

Skapa en konsollaplikation som skall agera som en enkel affär.
När programmet körs så ska man få se någon form av **meny** där man ska kunna välja att **registrera ny kund** eller **logga in**. Därefter ska ytterligare en **meny** visas där man ska kunna välja att **handla**, **se kundvagn** eller **gå till kassan**. 

Om man väljer att handla ska man få upp **minst 3 olika** alternativ att köpa (t.ex. Korv, Dricka och Äpple). Man ska se **pris** för varje produkt och kunna lägga till vara i **kundvagn**. 

Kundvagnen ska visa alla varor man lagt i den, styckpriset, antalet och totalpriset samt totala kostnaden för hela kundvagnen.
Kundvagnen skall sparas i kund och finnas tillgänglig när man loggar in.

När man ska Registrera en ny kund ska man ange Namn och lösenord. Dessa ska sparas och inte gå att ändra.

Väljer man Logga In så ska man skriva in namn och lösenord. Om användaren inte finns registrerad ska programmet skriva ut att kunden inte finns och fråga ifall man vill registrera ny kund. Om lösenordet inte stämmer så ska programmet skriva ut att lösenordet är fel och låta användaren försöka igen.


Både kund och varor skara separata klasser med **Properties** för information och metoder för att räkna ut totalpris och verifiera lösenord.

Exempel:
```cs
    public class Kund 
    {
        public string Name { get; private set; }

        private string Password { get; set }

        public Kund(string name, string password)
        {
            this.Name = name;
            this.Password = password;
        }
    }
```

Pro

## Redovisning
Uppgiften ska lösas individuellt eller i par. </br>
OBS! Väljer man att jobba i par skall man arbeta i samma repository.
Det skall vara tydligt vem som gjort vad.
Lämna in uppgiften på ithsdistans med en kommentar med github-länken. </br>

## Betygskriterier 
### För godkänt:
* Alla klasser ska vara publika.
* Koden ska fungera enligt ovan beskrivning.
* Man ska kunna få ut korrekt mittpunkt, area, omkrets (2D) och volym (3D)
på samtliga geometriska figurer (enligt ovan).
* .IsSquare och .IsCube ska korrekt ange om det är en kvadrat eller kub.
* Båda versionerna av GenereteShape ska fungera korrekt.
* ToString() ska vara implementerad så att alla shapes skrivs ut korrekt.
* Projektet som använder klassen ska ta fram en lista med 20 random objekt,
skriva ut alla objekten, samt trianglarnas total omkrets, alla objekts
genomsnittliga area, och ange det objekt med störst volym. 
### För väl godkänt krävs även:
* Koden ska vara väl strukturerad och lätt att förstå
* Lösningen ska inte innehålla massa onödig kod.
* Man ska även implementera extrauppgiften enligt nedan (IEnumerable). 

# OBS! Extra uppgift som krävs för VG! 

# Inlämning sker före deadline.
