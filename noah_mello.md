2/9
notes in this file as demonstrated by my instructor:
File Paths:
    Absolute start with /, inlcudes all directories between root and current
    Relative - start with .(current), ..(back), or ~(home), specifies location of a file relative to current
 Some Commands: 
    pwd - shows current terminal
    man [] - manual
    [] -h - help with that command
    ls - list, with -F (shows / to separate directories and * on ends of scripts), with -a (show hidden files), with -l (additional info)
    clear - clear the terminal
    cd - change directory, move current directory to wherever you say
    echo - repeat what you type

2/16
Some commands
    mkdir [name] - make directory with name []
    mkdir [name1]/[name2]/etc - make directory 2 within directory 1
    mkdir -p [name],[name] - make directories if parents dont exist
    rmdir - remove directory
    mv - move file (can be used to move, rename, or both)
        ex: mv bad_name good_name      - renames it
            mv ../notes.txt ~/notebook  - rename and move
            mv /tmp/data . move file to current directory
    cp - copy, with -R for directory, works like mv
    touch - creates a file
    rm - remove files/directories PERMANENTLY,
        need -R for directories
    cat - combine files (and view)
    > - redirect output of command to file, overwriting
    >> - redirect output to file, adding to it
    head - show first 10 lines of file
    tail - show last 10 lines of file
        both with -n[] to show only [] amount of lines
    ctrl + c - cancel command if its running a lot
    * - wildcard, will match any characters
    ls | wc - number of stuff
    

LAB 3 - Exercises
    3a. Ways to change directories 
        1. cd
        2. cd ~
        3. cd../../..
    3b. How many programs in /bin
        1922 Files
    1. Commands to find files with letters
        1. ls c*
        2. ls *a*
        3. ls *o
        Bonus. ls *a* *c*
    3c. Command used to find .fastq files
        1. ls /home/users/ntm1021/gen711-811/shell_data/untrimmed_fastq

2/23
less: scrollable file viewer
    suitable for large files or long lines
    Scroll with arrows, Q to exit, G to end, g to beginning
nano: text editor
    suitable for quick edits
    Ctrl+X to exit
*: wildcard command
    can match any character or amount of characters
grep: useful for finding contents with given term
    syntac follows: grep (term) (pattern) (files)
    -B (#) before, -A (#) after
    -o prints oly matching
    -v non matching
 stdin : input into a progra,
 stdout : output of a program
 Piping: forcing output of one command to be the input of another - uses |
 wc - word count, gives #lines, #words, #bytes
    with -l shows only lines, -w only words, -c only bytes
 Useful piping commands
 sort - sort lines of stdin, 
     with -h for readable numbers
 uniq - removed duplicate lines IF SORTED, 
     with -c shows how many ties that line occurred, -d to only print duplicates, and -u for only lines with no duplicates

3/1

cut - print selected parts of input based on tabs
    w/ -d [] changes delimeter from /t to []
    w/ -f [] selects [fields]
wget [url] downloads file from internet using HTTP
wget -0 [filename] [url] downloads and puts in output file
ls -l shows permissions
chmod - change mode, permissions of selected files
    w/ -r, recursive to all files in specified directory
target u: user, g: group, o: other, a: all 3
    +: add, -: remove
    r: read, w: write, x: exacutable
^c - kill running command
^z - pause running command
fg - continue paused command
bg - continue paused command in background
top - show running processes and resources used
q to quit
ps - show current running processes
    w/ -aux to show all processes on machine'

3/8

