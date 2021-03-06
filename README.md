# Kapitel 1: Diskussion om datorprogram.
Diskussion i klassen.

## Vad är ett datorprogram?

[Gå hit för att se svaret](svar/svar1.md)

## Kan du ge exempel på olika datorprogram?

[Gå hit för att se svaret](svar/svar2.md)

## Kan du ge exempel på olika saker som fungerar tack vare datorprogram?

[Gå hit för att se svaret](svar/svar3.md)

# Kapitel 2: Teori om datorprogram.
Lärarledd genomgång i klassen.

## Grunderna i ett vanligt datorprogram

![Grunderna i ett dataprogram](bilder/datorprogram.png)

## Hur skriver man ett datorprogram?

Datorprogram består av programkod (vanlig text som ser lite kryptisk ut). Programkoden berättar för datorn hur programmet fungerar. Precis som i vanligt skrivet språk, så finns det också olika programmeringsspråk, som alla ser lite olika ut.
Nedanför är exempel på hur man får datorprogram att skriva "Hejsan!", men i tre olika programmeringsspråk.
```
echo Hejsan!
```
```
printf("Hejsan!");
```
```
print "Hejsan"
```

## När något går fel i ett datorprogram
![När något går fel i ett datorprogram](bilder/fortnite.png)

När ett datorprogram inte fungerar som det ska, så säger man ofta att programmet har en `bugg`. Det är då för att personen som skrivit programmet har skrivit fel. Det är vanligt att ett datorprogram är tiotusentals rader med text och en del program är flera miljoner rader med text, så det är inte konstigt att det kan bli fel.

## Exempel från ett känt datorprogram

![Snapchat](bilder/snap-ghost-yellow.png)

Hur fungerar snapchat? Som ett vanligt datorprogram, i grunden. Det vill säga:
* Snapchat tar emot något
* Snapchat gör något med det som tagits emot
* Snapchat skickar ut något

Mer i detalj, det som händer är att:
* Du skriver något eller tar en bild. Snapchatprogrammet tar emot det.
* Snapchatprogrammet ser till att din bild ser extra skoj ut eller lägger till emojis i din text.
* Snapchatprogrammet skickar meddelandet till din kompis.

![Hur fungerar Snapchat](bilder/hurfunkarsnapchat.png)

# Kapitel 3: Skriv ditt eget datorprogram!

## Anslut till datorn som du ska programmera på
1. Du har fått ett papper där det står adressen till en webbsida. Gå till den.

2. Klicka på `Advanced` eller `Advancerat` som på bilden nedan.
![Hur man loggar in](bilder/first.png)

3. Klicka på `Fortsätt till...` eller `Proceed to...` som på bilden nedan.
![hur man loggar in](bilder/second.png)

4. Logga in med användarnamnet `student` och lösenordet `ribersborg` och klicka på knappen som läser `Log in`, som på bilden nedanför.

![Hur man loggar in](bilder/third.png)

5. Klicka på menyn till vänster som läser `terminal`. När du gjort det så kommer det se ut som på bilden nedanför.

![Hur man loggar in](bilder/skrivprogram.png)

## Skriv ditt första datorprogram
1. Nu är vi redan att skriva vårt första datorprogram, det är ett enkelt program som skriver en bit text. I den svarta delen av skärmen skriv nedan:
:exclamation: Du skriver `>` genom att trycka `SHIFT + knappen med < > och | på sig`.
```
cat >mittprogram
echo Hej världen, detta är mitt första datorprogram
```
2. Tryck sedan `ctrl+c`.

3. Skriv nedan på skrämen för att köra ditt dataprogram.
```
sh ./mittprogram
```
4. Se hur ditt datorprogram skrev ut det du bestämde på skärmen! Hurra :smile:

## Från och med nu så får du fritt pröva att skriva lite olika dataprogram. 
Nedan så följer lite exempel som du kan pröva.

:exclamation: Det är lätt att göra fel. Om det står något konstigt på skärmen, så pröva att skriva om texten igen. 

### Ett datorprogram som skriver lite olika texter
:exclamation: Du skriver `>` genom att trycka `SHIFT + knappen med < > och | på sig`.
```
cat >olika
echo Hejsan alla
echo Jag vet inte vad jag ska skriva här!
echo Här kommer ännu mer text
```
Skriv sedan: `ctrl+c` och `sh ./olika`.

### Ett datorprogram som skriver en text 5 gånger
:exclamation: Du skriver `>` genom att trycka `SHIFT + knappen med < > och | på sig`.
```
cat >flera
for i in 1 2 3 4 5
do
echo Är det inte rast än?
done
```
Skriv sedan: `ctrl+c` och `sh ./flera`.

### Ett datorprogram som skriver en text hela tiden, tills du trycker `ctrl+c`
```
cat >evigt
while true
do
echo Är det inte rast än?
sleep 1
done
```

### Ett datorprogram som frågar efter vad du gillar
:exclamation: Du skriver `>` genom att trycka `SHIFT + knappen med < > och | på sig`. Du skriver `"` genom att trycka `SHIFT+2`. Du skriver `$` genom att trycka `AltGr+4`.
```
cat >fråga
read -p "Vad gillar du mest?" SVAR
echo Jag gillar också $SVAR
```
Skriv sedan: `ctrl+c` och `sh ./fråga`.

### Mer advancerat: Ett datorprogram som frågar efter vad du gillar och om du gillar glass, så blir programmet extra glatt, annars inte...
:exclamation: Du skriver `>` genom att trycka `SHIFT + knappen med < > och | på sig`. Du skriver `"` genom att trycka `SHIFT+2`. Du skriver `$` genom att trycka `AltGr+4`. Du skriver `[` genom att trycka `AltGr+8`. Du skriver `]` genom att trycka `AltGr+9`.
```
cat >advancerat
read -p "Vad gillar du? " SVAR
if [ "$SVAR" == "glass" ]
then
echo Jag gillar också glass!
else
echo Jag gillar inte $SVAR :(
fi
```
Skriv sedan: `ctrl+c` och `sh ./advancerat`.

* Överkurs: Hitta på ett helt egna datorprogram :smile:
