echo prints anything that comes after it
echo "\"(Ôo)'" prints a confused smiley
cat /etc/passwd prints the contents of passwd
cat prints anything that comes after it
tail /etc/passwd list the last ten lines in passwd file
head /etc/passwd prints the first ten lines of the file passwd
head -3 iacta | tail +3 prints the thrid line of the file iacta
echo 'best school' >> \*\'Best School\'\*$\?\*\*\*\*\*:) creates a file containing best school
ls -la > ls_cwd_content writes the listed files gotten from ls -la into the file ls_cwd_content
tail -n 1 iacta iacta duplicates the last line
rm *.js deletes all js files in the current working directory
ls -1Ra counts the number of directories and subdirectoriea
ls -t | head -n 10 list the files in a directory according to the time they were edited
sort | uniq -u takes a list of words as input and prints only words that appear exactly once
grep -l root /etc/passwd displays the lines containing root
grep -c bin /etc/passwd displays the number of lines that contain the pattern bin in the file /etc/passwd
grep A- 3 root /etc/passwd Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd
grep -v bin /etc/passwd Display all the lines in the file /etc/passwd that do not contain the pattern bin
grep ^[a-zA-Z] /etc/ssh/sshd_config display lines starting with a character
tr Ac Ze Replace all characters A and c from input to Z and e respectively
tr -d Cc removes all letters c and C from input
rev reverses text input
find . -empty -printf "%f\n"  finds all empty files and directories in the current directory and all sub-directories
find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f lists all the files with a .gif extension in the current directory and all its sub-directories.
cut -c 1 | paste -s -d '' decodes acrostics that use the first letter of each line.
tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev 
Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
