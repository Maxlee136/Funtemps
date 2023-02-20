Jeg samarbeidet med Andreas oppgaven

Til tross for de ulike utfordringene som oppsto underveis, var oppgaven veldig lærerik og tvang oss til å finne kreative løsninger.

Filer som test, conv og funfacts var for det meste enkle å håndtere etter at vi forsto prinsippene bak dem. Vanskelighetene oppsto hovedsakelig i kodingsprosessen for main.go-filen, da det var utfordrende å få formatene riktig for outputen. Selv om vi ikke klarte å legge til funfacts-delen i main.go, er vi fortsatt fornøyde med sluttresultatet og det vi lærte i løpet av oppgaven.

Programmets formål er å konvertere temperaturer mellom Celsius-, Fahrenheit- og Kelvin-skalaer. Programmet tar innspill fra kommandolinjen og bruker flaggpakken til å analysere kommandolinjeargumenter. Programmet bruker også to eksterne pakker conv and funfacts.

Conv-pakken gir funksjoner for å konvertere temperaturer mellom forskjellige skalaer. . Programmet har følgende kommandolinjeflagg:

- F: temperatur i grader Fahrenheit
-C: temperatur i grader Celsius
-K: temperatur i grader Kelvin
-out: utgangstemperaturskalaen kan være enten C (Celsius), F (Fahrenheit) eller K (Kelvin)

Funksjonen init() initialiserer kommandolinjeflaggene. Main()-funksjonen analyserer kommandolinjeflaggene ved å bruke flag.Parse()-funksjonen og utfører deretter de nødvendige temperaturkonverteringene. Programmet er bygd opp av diverse if-else-setninger som sjekker for gyldige flaggkombinasjoner og utfører de nødvendige temperaturkonverteringene.

Hvordan utfører du koden på din maskin?

1. Klon Github repository (sørg for at du har go installert på pcen ellers funker ikke programmet)
2. Sørg for at GO root er initialisert

Sørg for at GO111MODULE = on dette gjøres ved kommando

`go env -w GO111MODULE=on`

bruk f.eks go run main.go -k da vil du få konverteringen for kelvin

C float
temperatur i grader celsius
-F float
temperatur i grader fahrenheit
-K float
temperatur i grader kelvin
-funfacts string
"fun-facts" om sun - Solen, luna - Månen og terra - Jorden (default "sun")
-out string
beregne temperatur i C - celsius, F - farhenheit, K- Kelvin (default "C")
-t string
bruker setter input verdi, hvis ikke setter programmet til deafult verdi Celsius (default "C")

`go run main.go -C 50 -out K`

da vil vi i dette tilfellet konvertere 50 celius om til kelvin

Terminal output:

Funtemps % go run main.go -C 50 -out K
0 K sun
len(flag.Args()) 0
flag.NFlag() 2
true
50 °C = 323.15 °K

‌
