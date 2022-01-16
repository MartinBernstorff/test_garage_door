# Framing of ML problems - Lauritsen 2021
But very few machine learning models in healthcare are tested prospectively and clinically deployed [1–4].

the effect of censoring on risk predictions [5]

> Many aspects of the emerging AI technology are yet unknown to the end-user, the healthcare professional, who needs to comprehend the AI technology to ensure a genuine clinical translation.

> Could possibly lead to high false-positive rates and associated fatigue of the end-user. Real clinical translation can only be reached if this fatigue is avoided

## Methods
CROSS-tracks cohort, population based, open cohort
Primary and secondary healthcare partners
18+ Horsens Regionshospital. 
Sep 1 2012 til December 2018, 18+, hospitaliserede.
Skal være > 24 timer og < 50 dage.

The included admissions were distributed across 13,134 unique residents. The prevalence of sepsis among these admissions was 6.25%.

Udfald:
Mistanke om infektion
	1. Samples for culture +
	2. Antibiotika indenfor 72 timer efter eller 24 timer før.
*og*
	1. delta-SOFA på ≥ 2 point fra 48 timer før til 24 timer efter mistanke om infektion

![](BearImages/3756004E-6E43-46D5-BFEF-76FD87E9E5B6-7959-00001265B4450276/E2B783AE-6C3E-4355-89CD-A37C27935880.png)

![](BearImages/A81345D7-69CF-473A-A1A2-4C885E0A616C-7959-0000126A868142F9/CB54129B-AD08-45F6-9CB3-F1D38FF3F53D.png)

XGBoost, typisk en ensemble af decision-trees.

![](BearImages/5C82DC7D-30BE-427A-A2C8-CA727EC1854A-7959-000012C0BB96E296/17F1C9E5-FAA0-4B26-8641-920F99202A87.png)

![](BearImages/57800D02-0714-43FC-9A4F-C7A41AECC41D-7959-00001427E9837622/4BF1BEA4-32C6-4D64-B699-1A0D7B4865C9.png)


Hvad er AUROC?
![](BearImages/ED17A33B-91ED-447E-BCE8-AEDB11458B0E-7959-000012D630CF6119/1280px-Roc-draft-xkcd-style.svg.png)
Hvor TPR = sensitivitet = recall og FPR = 1-specificitet

Hvad er AUPRC?
![](BearImages/B197C9A9-D87F-453E-8138-5D9973801C87-7959-000012F25B2B5A1F/a-Example-of-Precision-Recall-curve-with-the-precision-score-on-the-y-axis-and-the.png)
Hvor “precision = PPV” og “recall = sensitivitet”

AUPRC inddrager derfor prævalensen af udfaldet i ens dataset, men inddrager ikke “sandt negativer”. Hvis sens og spec er uændrede og > prævalensen, vil AUPRC blive større når prævalensen bliver større.

Og hvad er SOFA-scoren så?
*Bevidsthedsniveau (GCS)*
*Respiration*
*Kredsløb*
*Levertal*
*Nyretal*
*Thrombocytter*

![](BearImages/051F0091-A195-4DF6-8E0F-56C4C2395B0C-7959-000013354AA8BEA0/6F7FE3AF-B98A-4878-9D94-6D1E97236116.png)

De faktorer er, ikke så overraskende, også de faktorer der har de største mean[SHAP].

SHAP er et udtryk for, i hvor høj grad en given feature påvirker prædiktionen.

![](BearImages/98B09946-F3A3-4A75-AB2A-CD537FAC18A2-7959-00001396B5FE8195/51306152-4108-430A-BF67-BD1DEE4EBCC1.png)

<!-- {BearID:E8DB78FA-B4C0-480C-8E1B-F4751E2E03CA-7959-000011CAF04F2EE8} -->
