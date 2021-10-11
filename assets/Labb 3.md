# Lab3 – Quiz game!

Du har fått i uppgift att skapa ett grafiskt quiz-spel.</br>
Man ska kunna spela, editera befintligt eller skapa nytt quiz.</br>
Att editera, spela och skapa skall vara separata vyer (UserControls).</br>
Ett quiz skall innehålla flera flervalsfrågor med 3 svarsalternativ till varje fråga. Och sparas som XML, JSON eller CSV. Quiz-filerna skall sparas i appdata/local/"appens namn" 

Det skall finnas en klass för **Question** som har följande properties:
```cs
public string Statement { get;}
public string[] Answers { get; }
public readonly int CorrectAnswer { get; }
```
Det skall finnas en klass för **Quiz** som har förljande properties:
```cs
public ICollection Questions { get; }
public string Title { get; }
```
Och följande metoder:

```cs
public Question GetRandomQuestion()
```
```cs
public void AddQuestion(string statement, params string[] answers, int correctAnser)
```
```cs
public void RemoveQuestion(int index)
```

När man spelar spelet skall frågorna slumpas fram och man ska kunna se totala andelen och antalet korrekta svar efter varje fråga.

## Redovisning
Uppgiften ska lösas individuellt.

## Betygskriterier 
### För godkänt:
* Koden ska fungera enligt ovan beskrivning.
* Programmet skall fungera utan krasch.
* Både att spara och läsa fil skall ske asynkront.
* Både Quiz och Question skall ha lämpliga konsatruktorer.
### För väl godkänt krävs även:
* Koden ska vara väl strukturerad och lätt att förstå
* Lösningen ska inte innehålla massa onödig kod.
* Det ska vara skalbart och enkelt att utöka.
* Man ska även implementera extrauppgiften enligt nedan. 

## OBS! Extra uppgift som krävs för VG! 

Som extra uppgift vill kunden gärna ha följande extra funktionalitet:

* Frågor ska kunna ha bilder kopplade till sig.
* Quiz skall sparas i JSON-format.
* Frågorna skall vara ordnade efter ämne så att man kan välja att visa slumpade frågor från antingen ett eller flera ämnen.

# Inlämning sker före deadline.
