Create a script that will perform the following actions: Replace every instance of 'cat' in "infile" with 'dog'. Replace every instance of 'Navy' in "infile" with 'Army'. Replacements are case-sensitive. Write the output to the file specifed by the variable 'outfile'. function q1() { #Valid Variables are: infile=$1 outfile=$2

```
newfile=$1
filedate=$2
touch $newfile
touch -t ${filedate}1730 $newfile
```
Create a script that will perform the following actions: Print to standard output the total number of files in the directory specified by dirname. If the directory does not exist, print 'Invalid Directory' The count excludes the '.' and '..' pseudo-directories. function q1() { #Valid Variables are: dirname=$1 #Your code here }

```
count=$(ls -1 $dirname | wc -l)
if [[ $count -gt 0 ]]; then
  echo $count
else
  echo Invalid Directory
fi
```
