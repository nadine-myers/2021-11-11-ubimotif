# Unix commands from the workshop

commands (BASH shell — most basic shell)

* whoami
* date
* pwd (present working directory)
* ls (show content of folder you are in)
* cd Desktop (change directory to the desktop)
* pwd (confirm desktop is directory)
* ls (show stuff on desktop)
* mkdir 2021-11-11-ubimotif (make a folder on the desktop)
* ls (show your new folder you made)
* cd 2021-11-11-ubimotif (to move to this directory)
* cd - (moves you back to Desktop)
* cd - (two times, moves you back to your old folder, a way to jump between two folders)
* cd .. (moves you back a folder)
* ls -F (shows folder files via / symbol)
* ls -a (shows hidden files)
* man ls (opens ls manual; can also google online if it is unclear)
* ls

## Numbered list of some commands
1. cd Desktop/shell-lesson-data (go to the shell lesson data directory)
2. if you are ALREADY in the Desktop, then type cd shell-lesson-data
3. ls (check whats in there)

## Checkbox list
* [x] ls -a
ls -F
less notes.txt (we want to look at this file)
Q (quit the file)
less numbers.txt
less (command to read a file, but not using all your memory to open the entire thing)
pwd (/Users/msharan/Desktop/shell-lesson-data -- this an absolute path)
ls -tlr (all items on desktop, sorted by time, with long name, in reverse order)
pwd
mkdir (make a folder)
mkdir 'notes and stuff' (quotations enable use of spaces)
cd ../.. (go back up two levels up)
ls / (list all folders)
ls /Users/fredastaire/Desktop/shell-lesson-data (list all items in that folder)
ls -art (all files, in reverse, according to time)
nano blabla.txt (command to create a file i.e. blabla.txt)
ctrl + O (to save the file)
ctrl + X (to exit file)
mv blabla.txt DONTOPEN.txt (function one of mv -- to rename something)
mv DONTOPEN.txt ../trash (function two of mv -- move something to the trash folder above)
cp (copy command ONLY FOR FILES)
rm (remove command)
always ls to check whats in there
touch EMPTY.txt (to create an empty file)
cp -r trash (copy command FOR FOLDERS)
rm -ir trash/
mv data 2021-11-11-ubimotif

Unix commands that we planned to teach

pwd
whoami
date
ls
ls -F
pwd
root directory
Meaning of /, @
cd
ls
cd Desktop
clear
ls -F
ls --help (windows)
man ls (mac/linux)
unsupported flags (lf)
ls -r
ls shell-lesson-data
mkdir 2021-11-11-ubimotif
cd 2021-11-11-ubimotif
ls
cd ..
pwd
ls -F -a
cd -
cd ~
absolute vs relative path: ., .., ~
ls ~/Desktop/shell-lesson-data
prompt $ + command (ls) + option (-F) + argument/filepath (.)
cd Desktop
mv shell-lesson-data 2021-11-11-ubimotif
mv data 2021-11-11-ubimotif
ls 2021-11-11-ubimotif
cd 2021-11-11-ubimotif/shell-lesson-data
cd creature
Tab completion
mkdir thesis
mkdir thesis/input thesis/output
naming convention
Creating a text file: touch, less, nano, less, upper Tab
cp notes.txt thesis
ls
cp vs mv
less numbers.txt
cp numbers.txt thesis/input/numbers-data1.txt
less thesis/input/numbers-data1.txt
mv thesis/input/numbers-data1.txt thesis/input/numbers-data.txt
cp vs mv
rm thesis/input/numbers-data.txt
rm -i thesis/input/numbers-data.txt
cp data/amino-acids.txt data/planets.txt thesis/input
cp data/pdb/* thesis/input
cp -r data/* thesis/input
cd thesis/input
ls *.pdb
ls *ane.pdb
less cubane.pdb
wc cubane.pdb (lines, words, and characters)
wc *.pdb
wc *.pdb > file_lengths.txt
less file_lengths.txt
cat file_lengths.txt
sort numbers.txt
sort -n numbers.txt
sort -n file_lengths.txt
sort -n file_lengths.txt > sorted_file_lengths.txt
head -n 1 sorted_file_lengths.txt
head -n 5 sorted_file_lengths.txt
head -n 5 sorted_file_lengths.txt > saving_output.txt
less saving_output.txt
head -n 1 sorted_file_lengths.txt > saving_output.txt
less saving_output.txt
head -n 5 sorted_file_lengths.txt >> saving_output.txt
less saving_output.txt
echo "appending more lines"  >> saving_output.txt
less saving_output.txt
head -n 5 sorted_file_lengths.txt | sort -r | head -n 1
head -n 5 sorted_file_lengths.txt | tail -n 1
cat animals.txt
cut -d , -f1 animals.txt
cut -d , -f2 animals.txt | sort
cut -d , -f2 animals.txt | sort > sorted-animals.txt
