# Pandas: Scatterplot
```
data.plot(kind="scatter", 
	x="longitude", 
	y="latitude", 
	alpha=0.1, 
	s=data["population"]/100, 
	label="population", 
	figsize=(10,7), 
	c="median_house_value", 
	cmap=plt.get_cmap("jet"), 
	colorbar=True)
```

<!-- {BearID:6E358C48-EF7A-40B4-8934-F209EFD23C4D-93658-000001966EDFF9B9} -->
