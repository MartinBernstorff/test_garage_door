# DAG-code
dag {
"Medication use" [outcome,pos="-0.512,-1.001"]
"Psychiatric diagnosis" [pos="-0.382,-1.016"]
"Psychiatric disease" [pos="-0.383,-1.028"]
"Shared base processes" [pos="-0.507,-1.031"]
"Somatic diagnosis" [pos="-0.637,-1.015"]
"Somatic disease" [pos="-0.637,-1.027"]
MHC [exposure,pos="-0.509,-1.019"]
"Psychiatric diagnosis" -> "Medication use"
"Psychiatric disease" -> "Psychiatric diagnosis"
"Psychiatric disease" -> MHC
"Shared base processes" -> "Psychiatric disease"
"Shared base processes" -> "Somatic disease"
"Shared base processes" -> MHC
"Somatic diagnosis" -> "Medication use"
"Somatic disease" -> "Somatic diagnosis"
"Somatic disease" -> MHC
MHC -> "Medication use"
MHC -> "Psychiatric diagnosis"
MHC -> "Somatic diagnosis"
}

## Backlinks
* [[Rejected: Does MHC have direct effects on medication use]]
	* ![[Pasted image 3 1.png]]

<!-- #service -->

<!-- {BearID:5BBD0E22-ECE5-4282-B0E1-123013D4310A-15756-0000130BA3B2281C} -->
