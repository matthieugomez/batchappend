## description


The command `batchappend`  handles variables with conflicting types by converting them to string. The issue with the base command `append` is that variables with conflicting types are converted to  missing values.

## installation

```
net install batchappend , from(https://github.com/matthieugomez/stata-batchappend/raw/master/)
```

If you have a version of Stata < 13, you need to install it manually

1. Click the "Download ZIP" button in the right column to download a zipfile. 
2. Extract it into a folder (e.g. ~/SOMEFOLDER)
3. Run

	```
	batch ado uninstall batchappend
	net install capappend, from("~/SOMEFOLDER")
	```