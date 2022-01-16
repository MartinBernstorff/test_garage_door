# Targets (R)
GNU make for R.

Automatically monitors dependencies and only runs functions where either: 
1. The function has changed or
2. Its dependencies have changed

Can also monitor files – can it monitor sql?
 
* How does it handle the SQL pulls?
	* How much does it write down?

Advantages: 
* Saves time by only running that changed code - can't match interactive, but allows for faster knitting
* Encourages writing functions 

[[Targets markdown]]

## Backlinks
* [[10-Dec-21 - Review - Work]]
	* In general, running scripts of this size through a slow interface is just going to hurt. None of the current solutions ([[Targets (R)]], caching and knitting) are much better than a "Run all chunks". If anything, speeding up the code is probably the highest leverage.
* [[9-Dec-2021 - Review]]
	* Waiting for code to run. I think this project is nearing finalisation, but look into [[Targets (R)]] if undertaking basically anything in the future.

<!-- {BearID:D7D0DFEF-5172-4208-AECE-FEE1BA5001D3-931-0000000EF5E98857} -->
