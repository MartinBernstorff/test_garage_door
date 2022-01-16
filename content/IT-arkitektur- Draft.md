# IT-arkitektur: Draft
Hej XYZ!

Martin og Lasse her, fra Søren Dinesens ML-gruppe.

Indtil nu har vi fået lov til at arbejde på jeres servere, specifikt RMAPPS0892. Det har vi været helt enormt glade for at vi kunne gøre, på trods af at det var i forskningsøjemed, ikke drift.

Indenfor nærmeste fremtid får vi adgang til helt frisk hardware på Gødstrup. Det glæder vi os enormt til! 

Fordi hardwaren er til forskning, ikke drift, håber vi at vi kan få softwaren sat op, så den passer godt til os! Vi skriver til jer nu, så vi gør det så godt som muligt første gang.

Specifikt har vi 3 større ønsker:

*1. Mulighed for at skrive personfølsomme data lokalt*
Vi kommer til at have intermediære stadier i vores data-pipeline, som vil have enorm gavn af at vi kan skrive direkte til disken. Et glat workflow her vil gøre en kæmpe forskel for os. Når vi kommer på egen hardware tænker vi, at det kan klares med Windows folder level permissions. Vi skal opbevare data lokalt fra eksterne kilder (e.g. DST), der vil kræve lignende datasikkerhed.

*2. Lokal versionskontrol*
En instance med GitHub Enterprise eller lignende (f.eks. via en VMware instance) vil tillade os et enormt boost i programmeringseffektivitet, samtidigt med at vi maksimerer datasikkerhed. 

*3. R udenfor Conda-environments*
Det er sjældent at R-pakker shipper breaking changes, og vi har haft problemer med at starte R gennem conda-environments. Derfor vil vi gerne have installeret det udenfor disse. Skulle vi få bruge for environments kan de håndteres med renv gennem Rs projektfunktion.

De 3 ønsker vil væsentligt øge vores produktivitet fordi vi undgår fejl, og mindsker friktion og ventetid i udviklingen.

Hvis I har nogle ønsker fra os, så hører vi dem gerne!

Ovenstående er måske mere kompliceret! Derfor vil vi rigtig gerne mødes med jer til et møde ansigt-til-ansigt, hvor vi finder en god løsning for alle.

Mvh
Martin Bernstorff &
Lasse Hansen

<!-- {BearID:DB8C3242-4E66-4CC0-A7D6-49AAF5B26084-33413-0000059E1E7CE037} -->
