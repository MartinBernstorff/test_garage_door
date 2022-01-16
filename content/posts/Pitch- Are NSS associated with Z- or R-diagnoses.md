# Pitch: Are NSS associated with Z- or R-diagnoses
*The problem*
Are non-specific symptoms are treated appropriately in hospital? Ie. is referral to hospital helpful for non-specific symptoms? 

Many of the contacts in the NSS group are due to well-understood disease, but there are likely some that are due to worry about a symptom that doesn’t have a cause that the hospital can solve. If these are a large number, we should prioritise research into how to identify them before referral.

*Is the problem solved?*
After reviewing 200 titles and roughly 50 abstracts from `title:((non-specific) OR (medically unexplained) AND symptoms AND (adolescents OR children) AND hospital)` in PubMed, I found no literature on this.

*The solution*
If we assume that the NSS-group will have more referrals due to or promoted by NSS, we can use Z- and R-diagnoses as a proxy for “non-helpful” contacts. 

These are contacts which don’t lead to treatment, and thus most likely no improvement in the patients condition (under the assumption that the act of being examined isn’t helpful in the long run, eg. that it provides temporary relief but long-term worry, [[Diagnostic testing can lead to harm]]).

This can give us a lower-bound estimate of the potential for improvement ([[Are NSS handled well in the hospital?]]). If we could identify those that don’t benefit from referral before they reach hospital, there’s potentially a lot of money, time and suffering to be saved.

We can show these as both proportions of all contacts in each group, ratios and differences in counts pr. unit time.

If we split it by symptom, it also becomes an indicator of which symptoms we are the poorest at treating at hospital – if we had something to offer, we would not need a z- or r-diagnosis.

*Challenges/limitations*
* We don’t know the cause of the referral. We are checking whether a difference in referrals will be associated to NSS, ie. whether NSS is a useful indicator of risk for R- or Z-diagnosis. 
* If we find a difference, it may be due to a common cause of both NSS and R- or Z-diagnosis. However, I don’t have any good examples of this.
* Not all Z- or R-diagnoses are relevant here, eg. DR01 – Mislyd ved hjertet. This slightly decreases our power, and gives us some work filtering those out.
* Do we have sufficient power? In total, Z-diagnoses are: 26% of the somatic contacts, 13% of psychiatric contacts. R diagnoses are roughly 5% in each. I haven’t been able to find power-calculations for negative-binomial distributions, so haven’t been able to make informed decisions here.

*Does this solve the problem?*
If NSS are handled well in the hospital, we would expect a minor association to R- or Z-diagnosis, especially in comparison to the well-understood diagnoses.

We would also expect a relatively low KIP of Z- and R-diagnoses.

---
A strong difference would indicate that referral due to NSS typically doesn’t make much of a difference. To better examine that hypothesis, we could examine the proportion of ER contacts that results in a non-Z or -R diagnosis, as a proxy for “well understood diagnosis”, and compare that to our reference. We probably need to categorise them into groups to maintain sufficient power for this analysis.

<!-- #service/research-idea/4. pitchable# -->

<!-- {BearID:6A0DB97F-0D98-4F5C-8645-6033E22EC6B3-961-0000033F41EA6327} -->
