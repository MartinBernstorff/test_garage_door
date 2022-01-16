# Extract tags with context from notes to Airtable
This is an extension of [[$My note system]], allowing weighted random prompts to be sent to me via some system. It's a general implementation of the [[$Self-recommendations]], but now not only for things to read, but for actions more broadly.

I want it to:

* Go through notes
	* For each note
		* Add UUID to missing notes
		* Look for specific tags
			* If matched, connect to Airtable base table
				* If matching UUID, skip*
				* Else, add new record with
					* Note title
					* Full note content
					* Note excerpt
					* Match type (tag)
					* UUID
		* Remove records that represent a tag no longer found (eg. if the hashtag has been deleted from a markdown file)

Ideally, it should exhibit:
* [[Idempotency]]
	* Definitely required since I want to [[§Guide novelty search]], probably by recency
* [[Identity]]
	* The idea that I can update a record after it's been created. Probably also required! Can use the UUID function from Ankdown

## Backlinks
* [[$My research system]]
	* [[Extract tags with context from notes to Airtable]]
* [[Add RSS support to md extractor]]
	* This is an extension of [[Extract tags with context from notes to Airtable]].

<!-- #Life -->

<!-- {BearID:CBE96193-673F-4367-BB30-5B87BF38D4E2-15756-000013035FE0C369} -->
