# IT-infrastruktur
 Vi begynder så småt at have samlet nogle IT-arkitektur-ønsker, som vi rigtig godt kunne tænke os i Gødstrup.

 Og, måske endnu vigtigere, vil det gøre det til et meget sjovere stykke arbejde for de enormt talentfulde mennesker, vi gerne vil holde interesserede i projektet (e.g. Kenneth, de 2 nye CogScis).

Jeg skriver allerede nu fordi nogle af de tanker der kommer fra BI afspejler, at de allerede har workflows som de gerne vil have os til at passe ind i - noget som jeg selvfølgelig sagtens kan forstå!

Men for at undgå at vi i Gødstrup ender i et suboptimalt status-quo tænker jeg, at vi skal have italesat de her ting inden, der er lavet en "god-nok"-løsning. Jeg ved bare ikke, hvem vi skal sige det til? Lasse snakkede med Henrik (BI-arkitekten), og han anbefalede at spejle det setup der er nu, som for os vil lede til rigtig meget friktion!

Derudover leder det nuværende setup til en del problemer:
	* Mister R-kode (siden 23. september, så snart en måned siden fejlmelding)
	* Ingen versionskontrol
	* Nu en omvej at starte R-studio

Specifikt er de vigtigste ting:
	* Lokal version-control (github enterprise)
	* Et data-mæssigt hurtigt sted at skrive personfølsomme data til (en lokal SQL-server, eller et lokalt drev) – hvor vi ikke er begrænset af kun at måtte skrive X timer om dagen, eller at forbindelsen genstartes dagligt.

Teknisk burde det være muligt, når vi får egen hardware. – håber det åbner muligheder fordi vi ikke skal tage samme hensyn til drift.

* Mulighed for DST-sikkerhed.

* R udenfor Conda environment

* Skal vi bruge dødsårsager til udfald?

## Backlinks
* [[28/10/2021 - Møde om GPU og Gødstrup-infrastruktur]]
	* [[IT-infrastruktur]]

<!-- {BearID:899D7F03-F324-47B4-BB81-095C031C380B-81766-000004D610808C8D} -->
