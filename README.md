## description

When appending a bunch of `.dta` created from .`xls`, two variables may have the same name but differing types (string vs numerical). In this case, `append` throws an error. With the `force` option, `append` converts the string observations to missing values. 

Instead, in this scenario, the command `batchappend` converts the numerical observations to strings.

## installation

```
net install batchappend , from("https://raw.githubusercontent.com/matthieugomez/batchappend/master/")
```

If you have a version of Stata < 13, you need to install it manually

1. Click the "Download ZIP" button in the right column to download a zipfile. 
2. Extract it into a folder (e.g. ~/SOMEFOLDER)
3. Run

	```
	batch ado uninstall batchappend
	net install batchappend, from("~/SOMEFOLDER")
	```
