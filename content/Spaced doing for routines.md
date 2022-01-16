# Spaced doing for routines
For routine activities, I envision something like a linearly increasing probability around the ideal date.

0% prob at ideal date minus elasticity, 100% prob at ideal date plus elasticity

So 
`prob = (cur_date-start_date)/(2 * elasticity)`

In pseudocode, this means the app must do:
```
	get airtable information

	for routine in airtable information
		prob = (cur_date-start_date)/(2 * elasticity)
		if decide(prob):
			display 

	def display
		display text

		if input next:
			elasticity = elasticity * 1.1 // round up always here
		elif input increase interval:
			elasticity = elasticity * 2
		elif input yes:
			copy to clipboard
			next date = current date + interval
		elif input open:
			open airtable link

		push changes to airtable and show next
```

- But even for routines, some routines are week-based – eg. finding recipes for dinner needs to be done every weekend. I need to integrate that 
	- Periodical routines with a dropdown for the interval – every N days, weeks, months or years
	- Probably some with a date as well, eg. father's birthday

## Backlinks
* [[$Spaced doing]]
	* [[Spaced doing for routines]]
* [[Do sufficient maintenance]]
	* [[Spaced doing for routines]]

<!-- {BearID:40669689-F43B-4B3A-8272-F3B09EBC8621-27349-000019225CE8F1B2} -->
