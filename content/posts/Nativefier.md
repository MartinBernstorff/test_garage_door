# Nativefier
``` 
nativefier --name "NAME" "URL" --title-bar-style 'hidden' --internal-urls ".*(google|x)\.com.*" --user-agent "Mozilla/5.0 (Macintosh; Intel Mac OS X x.y; rv:42.0) Gecko/20100101 Firefox/74.0"
```

### Required to get past Google login screen
```
--user-agent "Mozilla/5.0 (Macintosh; Intel Mac OS X x.y; rv:42.0) Gecko/20100101 Firefox/74.0"
``` 
```--title-bar-style 'hidden'
	'hiddenInset'
	'customButtonsOnHover'
```

### For oauth:
API: https://github.com/jiahaog/nativefier/blob/master/docs/api.md
```
--internal-urls ".*(harvestapp|google|getharvest)\.com.*"
```
https://github.com/jiahaog/nativefier/issues/164

Icon
```
--icon "file"
```

<!-- {BearID:EBCC21D6-9735-4156-9AE6-30D2D9CECF61-43273-000085896EDFBEC5} -->
