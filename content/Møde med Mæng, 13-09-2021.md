# Møde med Mæng, 13/09/2021
## Introduktionsrunde

## Hvorfor? 
	* Prædiktion vs. causal inference
		* Meget epidemiologisk forskning bruger “stærk association” / “stærk prædiktor” til at hinte mod en spændende kausal faktor
		* Det kan vi også gøre her, men det er ikke det primære formål
	* Et “screeningsværktøj”

## Hvilke data har vi?
Alt registreret i MidtEPJ på psykiatriske patienter fra 2011 til 2020. Inkluderer somatisk information på disse.

Trækkes direkte fra BI, som har adgang til journaltekster.

Vi vil kun bruge data der kan findes i BI, da det er det der muliggør, at vi kan implementere i klinikken.

## Hvad kan vi?
* Udtrække information fra journaltekst
	* Mening af ord/tekst i kontekst (transformer-modeller, 2 cog. sci. PhD’er tilknyttet projektet)

* Træning af ML-modeller, i et framework der kræver væsentligt mindre variabel-selektion end klassiske modeller
	* Rangerer i kompleksitet fra logistisk regression til dybe neurale netværk

## Hvad vil vi?
Forbedre kliniske outcomes for psykiatriske patienter via beslutningsstøtteværktøjer.

Dilemmaet er som screening; hvornår, hvem og hvad der skal screenes for afhænger af, hvor god vores test er, og hvad konsekvensen af testen kan blive.

Derfor i princippet et 3-dimensionelt problem-rum, med mange mulige kombinationer. Vi har brug for eksperterne (jer) til at hjælpe os med at udforske det rum.

### Hvornår skal prædiktionen udføres?
Forestiller mig prediktioner genereret inden planlagte fysiske fremmøder; her er der mulighed for at handle på evt. faretegn.

* Detektere højrisiko-pt., der kan medføre yderligere udredning: 
	* Udredning (dyslipidæmi, hypertension, rygning, alkohol)
	* Præventive tiltag
* Potentielt detektere meget højrisiko-pt. nu, starter beh/grundig udredning (Holter, KAG?)

### Hvad?
Forestiller mig:

*Hjertet*
1. Akut iskæmi (AMI/CABG/PCI/trombektomi)
2. Kronisk iskæmi (ustabil angina, kronisk iskæmisk hjertesygdom)

*Hjernen*
1. Blødning
2. Iskæmi
3. Stroke UNS

### Hvor langt frem?
Vi har ca. 10 års opfølgningstid, så jeg tænker vi træner 2 modeller:
* 1 år frem i tid (til de mere akutte interventioner)
* 5 år frem i tid (imiterer mere SCORE2 el. lign.)

Det er dog ikke sat i sten. Måske man kan opdele problemet i 2 – prædiktere både (1) Klassificere event indenfor follow-up (binært) og (2) Regression på tid til event (kontinuert) #Collaborators/Lasse

### Next steps
Diagnose vs. Screening, under 40? 

Hvem? (Selekter på alder)

Amputationer?

Type 2 diabetes algoritme, Christopher Rohde

<!-- #service #p2 -->

<!-- {BearID:3B61FE1D-1D0B-4A77-9714-4C3F228D82A5-33067-00000144CC6D76BD} -->
