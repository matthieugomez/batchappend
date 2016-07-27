## description

When, between two datasets, two variables have differing types (string vs numerical), `append` throws an error. With the `force` option, `append` converts the strings to missing values. Instead, the command `capappend` converts the numerical variable to strings, without destroying information.

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
