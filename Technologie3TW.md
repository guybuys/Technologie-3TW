# Technologie (3TW)
## _Overzicht van de lessen technologie_

Dit is een overzicht van wat we tijdens de lessen gezien, gedaan en besproken hebben. 

## Les 1 
_3 september_

- TinkerCAD account gekoppeld aan de klas
- Project aangemaakt met Arduino Uno R3
- Het basisprogramma in **scratch** ontleed
- Het basisprogramma in **C++** (text) overlopen
- De functie van de code blokken **setup()** en **loop()** besproken

## Les 2 
_10 september_

- Vandaag hebben we onze Arduino Uno R4 wifi voor een eerst keer aangesloten
- **Zorg dat je je Arduino tegen volgend les hebt, anders kost het je punten!!!**
- We gebruikten [ledmatrix-editor.arduino.cc](https://https://ledmatrix-editor.arduino.cc/) om tekeningen te maken die op het Arduino "LED-matrix" scherm kunnen komen
- Je kan met het programma **_animaties_** maken, dat is een aaneenschakeling van _beelden_ die we **_frames_** noemen. In een animatie moeten voor deze frames een _tijdsduur_ specifieren. Dit gebeurt onderaan de kleine weergave van de frame. Standaard staat deze tijd op 66. Alle leerlingen hebben een animatie gemaakt.
- We kunnen de animatie exporteren door op het **</>** logo te klikken. Er wordt gevraagd een naam voor de animatie op te geven. Deze naam mag **GEEN** spaties bevatten.
- Er wordt een file met de ingegven naam met extentie .h in de Downloads folder geplaats. Je kan deze file openen met een tekst-editor zoals **Kladblok**, ** Notepad** of **Notepad++**

De file ziet er als volgt uit:
```C++
const uint32_t smile_animation[][4] = {
	{
		0xa,
		0x2,
		0x81100e0,
		666
	},
	{
		0xa,
		0x2,
		0x81f00e0,
		666
	},
	{
		0xa,
		0x3,
		0xf81100e0,
		666
	}
};
```
Dit bestand bevat een animatie met 3 frames. We bestudeerden de code-block van de animaties. De buitenste code-block, die de volledige animatie bevat, begint helemaal links met **const uint32_t smile_animation[][4] = {** en eindigd eveneens helemaal links met **};** 

In de code-blok, springt alles in met 4 spaties. Daar hebben we opnieuw 3 code-blokken die de frame (en zijn duurtijd) beschrijven. Deze code-blokken beginnen met een **{** en eindigen met **}**. Zolang het niet de laatste code-block is, wordt er een komma geplaats na de accolade die het einde van het block aangeeft. Dit wil zeggen dat er een nieuwe block gaat beginnen.

Ook in deze code-block, springt alles opnieuw 4 spaties in. Daar staan enkel getallen (met een notatie die we nog niet kennen). Zolang het niet het laatste getal is, staat er een komma achter om aan te duiden dat het nog niet gedaan is.

**Zorg dat je deze structuur goed begrijpt, volgende week doen we hier een test over**

Tenslotte hebben we geleerd hoe we een enkele **frame** kunnen maken uit een frame van een animatie. De 2 verschillen zijn dat er maar 1 code-block nodig is en deze code-block heeft geen _tijdsduur_ nodig.

In dit volgende voorbeeld hebben we een enkel frame gemaakt van eerste frame uit de animatie:

```C++
const uint32_t smile_frame[] = {
	0xa,
	0x2,
	0x81100e0
};
```

**Zorg dat je ook deze structuur goed begrijpt, ook hier komt een vraag in de test van volgende week**

## Les 3 
_17 september_

Test over de les van 10 september. 

## Les 4
_24 september_

Taak: maak een frame met uw initialen en een animatie

## Les 5
_1 oktober_

Deze les laden we de animatie en de frame met initialen uit de taak van vorige week in onze Arduino.
**Let op:** in 3TWb moeten de code in de IDE nog naar het Arduino bordje opgeladen worden. Zorg dat alles hiervoor klaar is, anders verlies je punten... 


**_Wordt vervolgd..._***
