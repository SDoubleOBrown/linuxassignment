# List of 15 file operators with explanations

## 1.   -r file

DESCRIPTION: Checks if file is readable.

EXAMPLE:
`if [ -r $file ]
then
   echo "File has read access"
else
   echo "File does not have read access"
fi`

## 2.   -nt and -ot

DESCRIPTION: Check if one file is newer or older than another.

`if [ myfile1.txt -nt myfile2.txt ]; then
    echo "myfile1.txt is newer than myfile2.txt."
fi`

## 3.   -x file

DESCRIPTION: Checks if file is executable.

EXAMPLE:
`if [ -x $file ]
then
   echo "File has execute permission"
else
   echo "File does not have execute permission"
fi`

## 4.   -n string

DESCRIPTION: Checks if the string is not empty.

EXAMPLE:
`if [ -n "$mystring" ]; then
    echo "mystring is not empty."
fi`

## 5.   -z string

DESCRIPTION: Checks if the string is empty.

EXAMPLE:
`if [ -z "$mystring" ]; then
    echo "mystring is empty."
fi`

## 6.   -h filename

DESCRIPTION: Checks if the file exists and is a symbolic link (for compatibility).

EXAMPLE:
`if [ -h mylink ]; then
    echo "mylink exists and is a symbolic link."
fi`

## 7.   -S filename

DESCRIPTION: Checks if the file exists and is a socket.

EXAMPLE:
`if [ -S mysocket ]; then
    echo "mysocket exists and is a socket."
fi`

## 8.   -z string

DESCRIPTION: Checks if the string is empty.

EXAMPLE:
`if [ -z "$mystring" ]; then
    echo "mystring is empty."
fi`

## 9.   -ef filename

DESCRIPTION: Checks if two files have the same device and inode numbers, i.e., are hard links to the same file.

EXAMPLE:
`if [ file1.txt -ef file2.txt ]; then
    echo "file1.txt and file2.txt are hard links to the same file."
fi`

## 10.  -w filename

DESCRIPTION: Checks if the file exists and is a writable device file.  

EXAMPLE:
`if [ -w /dev/sda ]; then
    echo "/dev/sda exists and is a writable device file."
fi`

## 11.  -t fd

DESCRIPTIION: Checks if the file descriptor is open and associated with a terminal.

EXAMPLE:
`if [ -t 0 ]; then
    echo "stdin is open and associated with a terminal."
fi`

## 12.  -k filename

DESCRIPTION: Checks if the file exists and has the sticky bit set.

EXAMPLE:
`if [ -k myfile.txt ]; then
    echo "myfile.txt exists and has the sticky bit set."
fi`

## 13.  -u filename

DESCRIPTION: Checks if the file exists and has the setuid bit set.

EXAMPLE:
`if [ -u myprogram ]; then
    echo "myprogram exists and has the setuid bit set."
fi`

## 14.  -S filename

DESCRIPTION: Checks if the file exists and is a socket.

EXAMPLE:
`if [ -S mysocket ]; then
    echo "mysocket exists and is a socket."
fi`

## 15.  -c filename

DESCRIPTION: Checks if the file exists and is a character special file.

EXAMPLE:
`if [ -c mycharfile ]; then
    echo "mycharfile exists and is a character special file."
fi`