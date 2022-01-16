# Log: Diagnosestabilitet på tværs af LPR2->LPR3
*11/01/2022*
Some problems! It seems I just count open sequences now. But the sequences aren't dependent on whether they share diagnoses. This means our outcome is "åbne forløb pr. patient", instead of "antal diagnoser pr. patient".

To get around that, we need to count how many unique diagnosis+patient combinations there are in each period as the numerator.

Maybe I'm counting the number of open sequences, rather than patients with an open sequence. 

To solve this, I want to collapse sequences that overlap and are from the same patient, so that they keep the lowest start date and highest end date.

This is only necessary if a patient can have more than one open sequence in a quarter. This is possible due to the padding. We can change this if we onyl count unique dw_ek_borger in open sequences! 

*10/01/2022*
I also want to have a better idea about the y-axis for the diagnostic stability paper. I would love to do # incident diagnoses / active patients, but because the ending of sequence isn't well-defined, I'm not sure that's possible. 

The current break we see is not explainable by our definition, but our definition isn't terribly easy to interpret either. We might just want to report number of new diagnoses pr. quarter in the entire cohort, and then accept that there will be a trend towards more diagnoses pr. quarter. This means we'll have to detrend for statistical testing, though, making that harder to interpret. ::It's also no longer at the "individual" level.::

I could define a patient as "active" if it's been no more than 3 og 6 months since their last visit. *That resembles the constructed sequences quite a bit, doesn't it?* 

Not quite - I didn't change the way I counted the results in the individual constructed sequences diagram. It still conditions on having at least one visit within the quarter. 

[How to count records with start date end date interval in R? - Stack Overflow](https://stackoverflow.com/questions/30990718/how-to-count-records-with-start-date-end-date-interval-in-r/55909192)

To do this:
1. Seems like I can reuse the "connected sequences" code, and then just change how I count them

* Why do the open_sequences drop markedly around 2021-04-01?

* How do I calculate the confidence intervals for events per person

<!-- #sp -->

<!-- {BearID:1E760C70-7CC8-4859-8AB9-1F5BB1274E1D-63716-000004115AF8B902} -->
