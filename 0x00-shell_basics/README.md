# Shell Basics

This repository contains a set of shell scripts that perform various basic tasks on a Linux system. Each script is designed to be short, two lines long, and follows specific requirements.

## Scripts

1. **0-current_working_directory**: Prints the absolute path name of the current working directory.

2. **1-listit**: Displays the contents list of the current directory.

3. **2-bring_me_home**: Changes the working directory to the user’s home directory.

4. **3-listfiles**: Displays current directory contents in a long format.

5. **4-listmorefiles**: Displays current directory contents, including hidden files, in the long format.

6. **5-listfilesdigitonly**: Displays current directory contents in long format with user and group IDs displayed numerically.

7. **6-firstdirectory**: Creates a directory named my_first_directory in the /tmp/ directory.

8. **7-movethatfile**: Moves the file betty from /tmp/ to /tmp/my_first_directory.

9. **8-firstdelete**: Deletes the file betty in /tmp/my_first_directory.

10. **9-firstdirdeletion**: Deletes the directory my_first_directory that is in the /tmp directory.

11. **10-back**: Changes the working directory to the previous one.

12. **11-lists**: Lists all files in the current directory, the parent of the working directory, and the /boot directory in long format.

13. **12-file_type**: Prints the type of the file named iamafile in the /tmp directory.

14. **13-symbolic_link**: Creates a symbolic link to /bin/ls named __ls__ in the current working directory.

15. **14-copy_html**: Copies all HTML files from the current working directory to the parent of the working directory, preserving newer versions.

## How to Run

To run any individual script, use the following command:

```bash
./script_name

To run all scripts at once, use the provided run_all script:
./run_all
