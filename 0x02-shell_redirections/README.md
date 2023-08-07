#!/bin/bash

# Script 0: Hello World
# This script prints "Hello, World" to the standard output.
echo "Hello, World"

# Script 1: Confused Smiley
# This script displays a confused smiley "(Ôo)' to the standard output.
echo "(Ôo)'"

# Script 2: Display /etc/passwd
# This script displays the content of the /etc/passwd file to the standard output.
cat /etc/passwd

# Script 3: Display /etc/passwd and /etc/hosts
# This script displays the content of the /etc/passwd and /etc/hosts files to the standard output.
cat /etc/passwd
cat /etc/hosts

# Script 4: Display Last 10 Lines of /etc/passwd
# This script displays the last 10 lines of the /etc/passwd file to the standard output.
tail -n 10 /etc/passwd

# Script 5: Display First 10 Lines of /etc/passwd
# This script displays the first 10 lines of the /etc/passwd file to the standard output.
head -n 10 /etc/passwd

# Script 6: Display Third Line of iacta File
# This script displays the third line of the file named "iacta" located in the working directory.
head -n 3 iacta | tail -n 1

# Script 7: Write ls -la Result to ls_cwd_content
# This script writes the output of the 'ls -la' command to the file 'ls_cwd_content'.
ls -la > ls_cwd_content

# Script 8: Duplicate Last Line of iacta File
# This script duplicates the last line of the file named "iacta" located in the working directory.
last_line=$(tail -n 1 iacta)
echo "$last_line" >> iacta

# Script 9: Delete .js Files
# This script deletes all regular files with a ".js" extension in the current directory and its subfolders.
find . -type f -name "*.js" -exec rm {} +

# Script 10: Display 10 Newest Files
# This script displays the names of the 10 newest files in the current directory, sorted from newest to oldest.
ls -t | head -n 10

# Script 11: Print Unique Words
# This script reads a list of words from input, prints words that appear exactly once, and sorts them.
sort | uniq -u

# Script 12: Display Lines Containing "root" from /etc/passwd
# This script displays lines from the /etc/passwd file that contain the pattern "root".
grep "root" /etc/passwd

# Script 13: Count Lines Containing "bin" in /etc/passwd
# This script counts the number of lines in the /etc/passwd file that contain the pattern "bin".
grep -c "bin" /etc/passwd

# Script 14: Display Lines Containing "root" and Following 3 Lines from /etc/passwd
# This script displays lines from the /etc/passwd file that contain the pattern "root" and the 3 lines following them.
grep -A 3 "root" /etc/passwd

# Script 15: Display Lines Not Containing "bin" in /etc/passwd
# This script displays lines from the /etc/passwd file that do not contain the pattern "bin".
grep -v "bin" /etc/passwd

# Script 16: Display Lines Starting with a Letter in /etc/ssh/sshd_config
# This script displays lines from the /etc/ssh/sshd_config file that start with a letter, including capital letters.
grep "^[[:alpha:]]" /etc/ssh/sshd_config

# Script 17: Replace Characters
# This script replaces occurrences of characters 'A' with 'Z' and 'c' with 'e' in the input.
sed 's/A/Z/g; s/c/e/g'

# Script 18: Remove Letters c and C
# This script removes occurrences of the letters 'c' and 'C' from the input.
tr -d 'cC'

# Script 19: Reverse Input
# This script reverses its input.
rev

# Script 20: Display Users and Home Directories
# This script displays all users and their home directories, sorted by users, based on the /etc/passwd file.
awk -F: '{print "User:", $1, "Home:", $6}' /etc/passwd | sort -k2
