## description


The command `capappend`  handles variables with conflicting types by converting them to string. The issue with the base command `append` is that variables with conflicting types are converted to  missing values.

## installation

```
net install capappend , from(https://github.com/matthieugomez/stata-capappend/raw/master/)
```

If you have a version of Stata < 13, you need to install it manually
Click the "Download ZIP" button in the right column to download a zipfile. Extract it into a folder (e.g. ~/SOMEFOLDER)
2. Run: (changing SOMEFOLDER with whatever you picked)
```
cap ado uninstall capappend
net install capappend, from("~/SOMEFOLDER")
```