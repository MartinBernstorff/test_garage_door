# Programming in dplyr
Q. When would you use double-curly brackets {{ in R?
A. When referring to a variable from a function argument inside a dplyr function, e.g:
![](BearImages/8F87660D-B5C6-46AD-814B-C8A332DE36AD-3579-00000023D95F1907/E55ED314-E282-4091-BEFD-A3F7E69F846D.png)

Q. You want to run a function on each row in dplyr (the function isn't vectorised). How might you do this?
A. 
```
df %>%
	rowwise %>%
	function() %>%
	unnest
```

Q. Why does this not work? 
```
df <- df %>%
     mutate({{x_col}} = detrend_fn({{x_col}}, ...))
```
A. Assignment with double curly requires “:=“,  otherwise R throws a syntax error due to curly braces left of assignment

Q. Why does this not work? 
![](BearImages/9F7DAC2E-1772-49D5-BC32-F71D82F93B90-61430-000005804B816493/image_1637330144896_0.png)
A. dplyr verbs do not take strings as input

If this is the case, how do we make programmable column titless?

Q. 
![](BearImages/C5F37D88-4F82-4861-AD6F-F4FB301B1102-61430-000005806B62DE9A/image_1637330144896_0.png)
This function call returns an error. How do you correct it?
A. Unquote “tre”

Q. This function call returns an error. Why is that?
![](BearImages/A33E9C39-5E58-4F96-8267-29F39456D7EB-61430-000005807C54FD5C/image_1637330353335_0.png)
A. Assignment with double curly requires “:=“,  otherwise R throws a syntax error due to curly braces left of assignment

Q. Why do you need to use “:=” here? 
![](BearImages/505C404C-B96E-4278-81AD-3A7B4CBA2CFF-61430-000005808AE9A8EA/image_1637330418884_0.png)
A. Assignment with double curly requires “:=“,  otherwise R throws a syntax error due to curly braces left of assignment.

Q. Why does this not work?
![](BearImages/F06F5AA6-C4D3-40F0-B962-71DDFA2813AE-7920-00000226528724E5/1509BF33-EA5E-403F-ABAB-BC0D1186D4C2.png)
A. You need to use `!!col_out_name` to mark that it should pull from variable names.

Q. The following code returns an error.
![](BearImages/009186AB-28E4-4F66-AA29-4C7BB331E6A3-7920-0000022692C9A9E4/B3B41B78-BA11-4669-B838-3CED567798D3.png)
How do you fix it?
A. 
![](BearImages/0F3DE9B6-E36A-4852-B549-9BA73B03FF07-7920-00000226A39A774F/E77DF6C9-D766-44F6-B7F2-83F84C9AD0FD.png)


<!-- #anki/deck/Programming #anki/tag/R -->

<!-- {BearID:63E4BE7F-EED6-4D33-8D63-D74F3C2B11D4-3579-0000002353922545} -->
