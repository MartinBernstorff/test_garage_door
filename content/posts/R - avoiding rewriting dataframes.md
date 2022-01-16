# R - avoiding rewriting dataframes
Q. How do you get the number of rows in a dataframe in R?
A.  `nrows(df)`

Q. Assume that the below operation cannot be vectorised. Why is this an antipattern in R?
![](BearImages/0AC6B221-D324-449F-AF4E-658397557400-98018-0000019C601C0D71/C6CFB289-212A-462A-B0C1-985F55082023.png)
A. When writing directly to a df, R has to duplicate the df and then garbage collect

Q. How might you rewrite this for better performance?
![](BearImages/9A2E429D-D239-4017-AB97-E63FD41208B8-98018-0000019C61C4418C/C40615A6-4797-4FBF-9A84-0F1DA8FCC79F.png)
A. 
![](BearImages/5B312860-7246-4382-8A86-E0A9FF4BEC4C-46373-0000077B0999FDA5/ABA95B89-BE18-4A1B-A005-F0E05573083D.png)


<!-- #anki/deck/Programming -->

<!-- {BearID:250DC036-D363-407F-B3EC-9DCB739525A9-98018-0000019AF7D37711} -->
