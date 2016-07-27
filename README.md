## description

When two variables have the same names between two datasets, but their types differ (string vs numerical), `append` converts the strings to missing values. Instead, the command `capappend` handles variables with conflicting types by converting both to string. 

## installation

```
net install capappend , from(https://github.com/matthieugomez/stata-capappend/raw/master/)
```

If you have a version of Stata < 13, you need to install it manually

1. Click the "Download ZIP" button in the right column to download a zipfile. 
2. Extract it into a folder (e.g. ~/SOMEFOLDER)
3. Run

	```
	cap ado uninstall capappend
	net install capappend, from("~/SOMEFOLDER")
	```
