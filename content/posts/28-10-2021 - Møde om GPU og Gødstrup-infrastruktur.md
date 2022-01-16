# 28/10/2021 - Møde om GPU og Gødstrup-infrastruktur
*Formålet med mødet*
Forventningsafstemning, når vi kan snakke os til tingene gør det det hele meget nemmere.

Vi er ikke sysadmins, og har stor respekt for, at der er meget vi ikke ved. Derfor har vi enorm brug for jer.

*Hvad vi ønsker os:*
* Drømmescenariet: Noget vi kan SSH'e ind i, så vi ikke behøver udvikle gennem Citrix. Kan gøres med Windows Server 2019, eller med en Ubuntu server på en virtuel maskine. Der findes også 2FA til dette.

* Mulighed for at have personfølsomme oplysninger lokalt
	* Så god GDPR-komplians som muligt
		* Brugerbegrænset adgang
		* Ideelt set logning
	* En SQL server? E.g. en PostgreSQL i en docker container?

* Versionskontrol, e.g. at hoste GitHub Enterprise
	* Tillader os desuden bug-tracking/issue management og code-review på samme sted
	* Ideelt tilgængeligt udenfor RMs netværk også, men det er en meget lille detalje

* Re: Datamængder. Hvad er latenstiden fra bestilling til implementering? Vi er mere begrænsede af kalendertid end finanser, så at købe mere lager er nok ikke en dårlig ide.

Vi vil også enormt gerne høre fra jer, hvordan I tænker samarbejdet fungerer bedst muligt!


* [[IT-infrastruktur]]

* [[IT-arkitektur: Draft]]

<!-- {BearID:A1606B62-7CFE-4B51-9BB1-40202012D7E7-43256-0000019D24E71BB6} -->
