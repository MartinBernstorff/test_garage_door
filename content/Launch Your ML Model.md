# Launch Your ML Model
1. Get your solution ready for production (plug into production data inputs, write unit tests, etc.).
2. Write monitoring code to check your system’s live performance at regular intervals and trigger alerts when it drops.
	* Beware of slow degradation: models tend to “rot” as data evolves.
	* Measuring performance may require a human pipeline (e.g., via a crowdsourcing service).
	* Also monitor your inputs’ quality (e.g., a malfunctioning sensor sending random values, or another team’s output becoming stale). This is particularly important for online learning systems.
3. Retrain your models on a regular basis on fresh data (automate as much as possible).

## Backlinks
* [[§Machine Learning]]
	* [[Launch Your ML Model]]

<!-- {BearID:3BEEFD18-76E9-4A25-8C8B-A988EB2EFF52-93658-0000017C1C0D2861} -->
