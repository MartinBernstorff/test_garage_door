# Should predictions trigger collecting more information
E.g. if the model predicts 10% risk of AMI within 5 years, but lacks:

1. Smoking status
2. Lipids
3. Blood pressure

Shouldn’t we then prompt clinicians to collect that information, so it can give a more qualified answer next time/on the next day? 

Probably yes! Ask Kenneth/Lasse how/whether we can implement this – e.g. can we use uncertainty in the ML-model as an indicator? 

It's easier for structured data, where we can point towards exactly which information is missing.

<!-- #Collaborators/Lasse -->

## Backlinks
* [[§PhD: Implementation of CVD prediction]]
	* *Which consequences does it lead to?*

<!-- #p1 #service -->

<!-- {BearID:D0E97BE7-1E94-438F-932A-53828314933E-57501-000002D56A90D642} -->
