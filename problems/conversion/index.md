# Temperatuurconversie

> **Individueel.**
>
> Samenwerken bij deze opdracht is niet toegestaan; het is prima om medestudenten en anderen om hulp te vragen, als het er maar niet op neerkomt dat iemand anders een deel van het werk voor je doet. Voorbeelden van "redelijke" en "onredelijke" manieren van samenwerken vind je in de studiewijzer.

## Temperaturen

Graden Celsius C en graden Fahrenheit F staan met elkaar in verband via `F = (18C + 320) / 10` en andersom `C = (10F - 320) / 18`. Een conversietabel kan er als volgt uitzien. Deze is op basis van de temperatuur in Celcius, en loopt van 0° tot en met 20°, in stappen van 5°.

|   C |   F |
| --: | --: |
|   0 |  32 |
|   5 |  41 |
|  10 |  50 |
|  15 |  59 |
|  20 |  68 |

## Implementatiedetails

**Voordat je gaat programmeren ga je pseudocode schrijven. Lees onderstaande details, bekijk de voorbeelden hieronder, en volg dan de instructies onder het kopje Getting Started.**

Schrijf, in een bestand genaamd `conversion.c`, een programma dat de gebruiker vraagt om de eenheid van temperatuur: `C` van Celsius of `F` van Fahrenheit. Vervolgens vraagt het programma om de begintemperatuur, de eindtemperatuur en de stapgrootte. Daarna wordt een nette tabel uitgeprint, met op iedere rij de gekozen temperatuur en de temperatuur in de andere eenheid.

- Gebruik `get_char` en `get_int` om de gebruikersinvoer op te vragen en `printf` om de tabel te printen.

- Het programma moet ook de kleine letters `c` of `f` accepteren als invoer. Vraag de gebruiker opnieuw om input als er iets anders dan `C` of `F` wordt gekozen, tot de gebruiker een juiste invoer geeft. Weet je nog welke loop het beste past bij deze situatie?

- Vraag de gebruiker ook opnieuw om input als de stapgrootte geen positief geheel getal is, tot de gebruiker een juiste invoer geeft.

- Je moet de getallen (en letters) rechts uitlijnen. De functie `printf` kan dit voor je regelen! Gebruik `printf("%3d", getal)` om een willekeurig getal zo te printen dat het 3 ruimtes inneemt. Is het getal bijvoorbeeld 9, dan worden er twee spaties uitgeprint vóór de 9.

- Zorg dat de uitvoer van je programma _exact_ is zoals in de voorbeelden hieronder. Dat maakt automatisch testen mogelijk, maar daagt je ook uit om geen shortcuts te nemen.

## Voorbeelden

Je programma moet uiteindelijk werken zoals in de voorbeelden hieronder.

    $ ./conversion
    Welke eenheid van temperatuur (C of F)? C
    Wat is de begintemperatuur? 0
    Wat is de eindtemperatuur? 20
    Wat is de stapgrootte? 5
      C |   F
      0 |  32
      5 |  41
     10 |  50
     15 |  59
     20 |  68

    $ ./conversion
    Welke eenheid van temperatuur (C of F)? F
    Wat is de begintemperatuur? 0
    Wat is de eindtemperatuur? 10
    Wat is de stapgrootte? 2
      F |   C
      0 | -17
      2 | -16
      4 | -15
      6 | -14
      8 | -13
     10 | -12

    $ ./conversion
    Welke eenheid van temperatuur (C of F)? F
    Wat is de begintemperatuur? 100
    Wat is de eindtemperatuur? 0
    Wat is de stapgrootte? 3
      F |   C

     $ ./conversion
    Welke eenheid van temperatuur (C of F)? v
    Welke eenheid van temperatuur (C of F)? F
    Wat is de begintemperatuur? 0
    Wat is de eindtemperatuur? 9
    Wat is de stapgrootte? -3
    Wat is de stapgrootte? 0
    Wat is de stapgrootte? 3
      F |   C
      0 | -17
      3 | -16
      6 | -14
      9 | -12

## Getting Started

- Maak een bestand `pseudocode_temp.txt` om je programma in stappen op te delen en die stappen ook weer op te delen. Begin hiermee:

      * Invoer
          * Celcius of Fahrenheit (geldige invoer: c/C/f/F)
          * Begintemp (geldige invoer: ...)
          * Eindtemp (geldige invoer: ...)
          * Stap (geldige invoer: ...)
      * Uitvoer
          * Optie 1:
              * Stap 1 van optie 1...
          * Optie 2:
              * Stap 1 van optie 2...

  Zorg dat je alle stappen zo precies mogelijk invult en ontbrekende stappen erbij zet. Vul ook in wat geldige waarden zijn voor elke invoer. Bespreek de pseudocode eventueel met een assistent en kijk of je nog iets mist.

## Hoe testen

Klaar? Geeft je code de juiste output voor de verschillende combinaties van invoer die mogelijk zijn? En hou je ook goed rekening met foutieve invoer? Als je denkt dat je klaar bent, dan zijn dat de eerste dingen om te checken.

Je kunt ook het volgende commando geven in de Terminal om de correctheid van je programma na te gaan. Zorg dat je altijd zelf ook compileert, fouten oplost en handmatig test, want deze tool is bij volgende vakken niet beschikbaar!

    check50 -l minprog/checks/2022/conversion

En je kunt alvast de stijl van je programma laten controleren op een paar aspecten die vaak misgaan. Die kun je dan verbeteren, maar dit is niet verplicht voor het inleveren van de opdracht.

    style50 conversion.c
