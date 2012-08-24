This script asks for and creates a folder with subdirectories named after information you provide. The subdirectories will be named like so:

CEShannon-CS600-WK1, while the files similarly will be named CEShannon-CS600-WK1.tex and CEShannon-CS600-WK1.bib. 

One file for a LaTeX document and one for BibTeX. The script will ask you for your name and class and will create enough folders for an 8 week Term. If you have less or more weeks in a Term simply edit the script mkdir command and change the amount of loops the while loop makes.

Add or remove directories from the below in the script, change dir names and so forth:

mkdir -v -p  "$CLASS/"{WK1,WK2,WK3,WK4,WK5,WK6,WK7,WK8};

Don't forget to change the increments in the while loop:

while [ $week -le 8 ]

If you have questions just post a comment and I will try and fix it or offer some help. This is my first bash script which is shameful as I have used Linux and Unix for over ten years.

If you don't already have a LaTeX template I would highly recommend Andr'e Miede's found on the CTAN website:

http://www.ctan.org/tex-archive/macros/latex/contrib/classicthesis/

Place your template wherever and then copy and paste the full directory path plus file name in script. For example:

\home\theShanMan\Documents\ClassicThesis.tex

The script will, "cat ClassicThesis.tex >> CEShannon-CS600-WK7.tex" for each file in each directory. 


