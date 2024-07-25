#05
Create a script that will perform the following actions: Replace every instance of 'cat' in "infile" with 'dog'. Replace every instance of 'Navy' in "infile" with 'Army'. Replacements are case-sensitive. Write the output to the file specifed by the variable 'outfile'. function q1() { #Valid Variables are: infile=$1 outfile=$2

```
newfile=$1
filedate=$2
touch $newfile
touch -t ${filedate}1730 $newfile
```
Create a script that will perform the following actions: Print to standard output the total number of files in the directory specified by dirname. If the directory does not exist, print 'Invalid Directory' The count excludes the '.' and '..' pseudo-directories. function q1() { #Valid Variables are: dirname=$1 #Your code here }

#06
```
count=$(ls -1 $dirname | wc -l)
if [[ $count -gt 0 ]]; then
  echo $count
else
  echo Invalid Directory
fi
```
#07
Read the file specified by fname and perform an action based on the contents of the file: If contents are 0 to 9, print "single digit" to standard output. If contents are 10 to 99, print "double digit" to standard output. If contents are 100 to 999, print "triple digit" to standard output. Otherwise, print "Error" to standard output. NOTE: There will only be one line of content in the file specified by fname. function q1() { #Valid Variables are: fname=$1 #Your code here }
