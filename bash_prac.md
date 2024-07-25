# 6
Create a script that will perform the following actions: Create a file specified by the name newfile. Set the file modified date to the value specified in filedate and time to '1730'. NOTE: filedate contains only a valid date in YYYYMMDD format, not a time. function q1() { #Valid Variables are: newfile=$1 filedate=$2 #Your code here }

```
newfile=$1
filedate=$2
touch $newfile
touch -t ${filedate}1730 $newfile
```
Create a script that will perform the following actions: Print to standard output the total number of files in the directory specified by dirname. If the directory does not exist, print 'Invalid Directory' The count excludes the '.' and '..' pseudo-directories. function q1() { #Valid Variables are: dirname=$1 #Your code here }

#6
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
