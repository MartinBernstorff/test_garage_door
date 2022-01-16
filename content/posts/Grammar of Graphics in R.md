# Grammar of Graphics in R
An R layer is defined by:
1. Data
2. Mapping
3. Statistical transformation (stat)
4. Geometric object (geom)
5. Position adjustment (position)

If you want to split up a graphic into multiple sub-graphics, use facet_wrap:
![](BearImages/ADEF630A-C68E-4C3B-8BF7-BB187FA64447-477-0000011243E3491F/08E7AA4C-4FF8-45A9-BA35-747BBFBADC44.png)
```r
ggplot(data = mpg, mapping = aes(x = displ, y = hwy)) +
  geom_point() +
  facet_wrap(~ class)
```

There are many  gloms! Some of the most frequently used:
![](BearImages/39DABCD4-60A0-4123-AC26-93FD4E06B889-477-000001528DD68756/8DB85D56-DFDE-4DFA-A3C0-7B797A5C151E.png)
```
geom_point(aes(x = x_var, y = y_var))
```

<!-- {BearID:00158C10-9F76-4A59-9790-20139BAF5F0A-477-0000007B66AFB53D} -->
