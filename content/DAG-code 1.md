# DAG-code 1
dag {
"Base processes" [latent,pos="-0.738,-1.152"]
"Hospital contacts" [pos="-0.781,-0.144"]
"Other symptoms" [pos="-0.485,-0.491"]
"Psychiatric disease" [pos="-0.280,-0.812"]
"Somatic disease" [pos="-1.410,-0.800"]
Diagnoses [outcome,pos="-0.788,0.068"]
MHC [exposure,pos="-1.068,-0.497"]
Medication [outcome,pos="-0.796,0.285"]
"Base processes" -> "Psychiatric disease"
"Base processes" -> "Somatic disease"
"Hospital contacts" -> Diagnoses
"Other symptoms" -> "Hospital contacts"
"Psychiatric disease" -> "Other symptoms"
"Psychiatric disease" -> MHC
"Somatic disease" -> "Other symptoms"
"Somatic disease" -> MHC
Diagnoses -> Medication
MHC -> "Hospital contacts"
}

## Backlinks
* [[Is the MHC flow in hospital generally appropriate]]
	* This is under the naive assumption that MHC can only be caused by a somatic or psychiatric disease:
[[DAG-code 1]]

<!-- #service -->

<!-- {BearID:3A7A7A18-126E-43BE-AAD2-46F68CD4A391-15756-0000130BA2F91F02} -->
